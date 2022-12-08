<script setup>
import { reactive } from "vue";

const player = reactive({
  audio: null,
  status: 0, // 0:loading 1:ready 2:playing 3:paused
  duration: 0,
  currentTime: 0,
  timer: 0,
  seeking: false,
  userSeeking: false,
});

const loadAudio = () => {
  player.audio = new Audio("https://cdn.pixabay.com/download/audio/2022/06/13/audio_54f6c2ba71.mp3?filename=dark-sad-ambient-piano-113208.mp3");
  player.audio.addEventListener("canplaythrough", (event) => {
    if (player.seeking) {
      player.seeking = false;
      return;
    }
    player.status = 1; // set flag to ready
    player.duration = player.audio.duration;
    player.currentTime = player.audio.currentTime;
  });
  player.audio.addEventListener("seeking", (event) => {
    player.seeking = true;
  });
  player.audio.addEventListener("play", (event) => {
    player.status = 2; // set flag to playing
    setProgressTimer();
  });
  player.audio.addEventListener("pause", (event) => {
    player.status = 3; // set flag to pause
    clearProgressTimer();
  });
  player.audio.addEventListener("ended", (event) => {
    player.status = 1; // reset flag to ready
    clearProgressTimer();
    setCurrentTime(0);
  });
};

function play() {
  player.audio?.play();
}

function pause() {
  player.audio?.pause();
}

function setProgressTimer() {
  clearInterval(player.timer);
  player.timer = setInterval(() => {
    if (player.userSeeking) return;
    player.currentTime = player.audio.currentTime;
  }, 1000);
}

function clearProgressTimer() {
  clearInterval(player.timer);
}

function setCurrentTime(newValue) {
  player.audio.currentTime = newValue;
  player.currentTime = player.audio.currentTime;
}

function formatTime(time) {
  const m = 60;
  const s = 1;
  const mod_m = time % m;
  const mod_s = mod_m % s;
  const mm = ((time - mod_m) / m).toFixed(0).padStart(2, "0");
  const ss = ((mod_m - mod_s) / s).toFixed(0).padStart(2, "0");
  return `${mm}:${ss}`;
}

loadAudio();
</script>

<template>
  <span>
    <template v-if="player.status == 0">music loading...</template>
    <template v-if="player.status == 1">music is ready.</template>
    <template v-if="player.status == 2">music playing...</template>
    <template v-if="player.status == 3">music is paused.</template>
  </span>
  <div>
    <input
      type="range"
      id="volume"
      name="volume"
      min="0"
      :max="player.duration"
      :value="player.currentTime"
      @change="setCurrentTime(Number($event.target.value))"
      :disabled="player.status == 0"
      @mousedown="player.userSeeking = true"
      @mouseup="player.userSeeking = false"
    />
    {{ formatTime(player.currentTime) }}/{{ formatTime(player.duration) }}
    <button v-if="player.status == 0" disabled>Loading...</button>
    <button v-if="player.status == 1" @click="play">Play</button>
    <button v-if="player.status == 2" @click="pause">Pause</button>
    <button v-if="player.status == 3" @click="play">Continue</button>
  </div>
</template>