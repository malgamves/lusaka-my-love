<template>
    <main @scroll="playSound">

        <section class="white">
            <div class="row-left">
                <p>  ☁☁  ☁  ☁  ☁  ☁    </p>
                <br>
                <p>  ☁☁☁  ☁  ☁  ☁  </p>
                <p>  ☁  ☁  ☁  ☁  ☁  </p>
                <p> ☁  ☁  ☁  ☁   </p>
                <br>
                <p>  ☁  ☁  ☁  ☁  ☁   </p>
                <p>  ☁  ☁  ☁  ☁  ☁  </p>
                
            </div>
            <div class="row-left">
                <p>  ˈ       ˈ </p>
                <br>
                <p>  ˈ </p>
                <p>  ˈ </p>
                <p> ˈ </p>
                <br>
                <p>  ˈ  </p>
                <p>  ˈ </p>
            </div>

            <div class="row-left">
                <p>  ˈ   .    ˈ      .</p>
                <br>
                <p>  ˈ </p>
                <p>  ˈ </p>
                <p> ˈ </p>
                <br>
                <p>  ˈ  </p>
                <p>  ˈ </p>
                
            </div>

            <div class="row-left">
                <p> lusaka, my love </p>
                <br>
                <p> the place i never got to </p>
                <p> know but am defined by </p>
            </div>

            <div class="row-left">
                <p> lusaka, my love </p>
                <br>
                <p> the place i never got to </p>
                <p> know but am defined by </p>

            </div>
            <button v-if="!isAutoplay" @click="setAutoplay"> hi </button>
            <button v-else @click="stopAutoplay">bye</button>

        </section>

        <section class="white">
            <div class="row">
                <img src="https://i.imgur.com/MLDDpTV.png" alt="">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>
                    <p> wild heards beat for the plains that nurtered them, til the thing that kept them alive stops
                        their breathings.</p>
                    <br>
                    <p>it hurts to leave but will i ever know anything outside your sheltered streets and tiny store</p>
                    <br>
                    
                    <hr>

                </div>
            </div>

        </section>



        <section class="white">
            <div class="row">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>
                    <p> it hurts to leave but i do because when i hear melissa i think about thier bread, i heard they
                        burned down and i waasn't there to talk about how tragic it might be to stay stuck when i could
                        swim in the oceans</p>
                        <br>
                    <p> it hurt to leave but i had to grow, the one thing that didn't thrive in that mild savanna was my
                        will to live.</p>
                    <br>
                    

                </div>
                <img src="https://i.imgur.com/3PJtQ93.png" alt="">
            </div>

        </section>

        <section class="white">
            <div class="row">
                <img src="https://i.imgur.com/8jhvOHY.png" alt="">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>
                    <p>i always liked purple, i mourned your trees and how they stripped your character to make way for
                        a struggling nations version of suburbia.</p>
                    <br>
                    <p>"the middle class is dead" i said as i looked around, my works a larger sign of what i lost</p>
                    <br>

                    


                </div>
            </div>

        </section>



        <section class="white">
            <div class="row">
                <div>         
                               <h3> ꙰    ☁ part 1, the end</h3>
                               <p> kids to get class they just don't know what to call it, they never teach that in school, nuance
                                isn't a path for a boy whose sheltered upbringing painted his world view</p>
                            <br>
                            <p>when i did leave i loved it, you became a place that kept things dear to me, my keys, my cards, a
                                bracelet, my shells, a medal, photos, my heart</p>
                            <br>
                            
                </div>
                <img src="https://i.imgur.com/VJM8v2Z.png" alt="">
            </div>

        </section>

        <section class="white">
            <div class="row">
                <img src="https://i.imgur.com/dHfQQRg.png" alt="">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>

                    <p> hard to grow away from your heard, it keeps you going to places in search of nothing.. i did
                        feel it again when i visited or when friendship turned to love, then i lost you again at this
                        isn't working out</p>
                        <br>
            <p> you were there for me then, you gave me hope and sheltered me as i planned to leave you again
            </p>
            <br>
            
                </div>
            </div>

        </section>



        <section class="white">
            <div class="row">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>

                    <p> i remember sitting in my moms garden starring at your blue skies, how i miss that view now</p>
            <br>
            <p> hard to think about love when it comes and goes</p>
            <br>

                    <p>we chose the life we think we deserve so i lived life and you made me feel alive</p>
                    <br>
                </div>

                <img src="https://i.imgur.com/nlpCLDp.png" alt="">
            </div>

        </section>

        <section class="white">
            <div class="row">
                <img src="https://i.imgur.com/um9kn81.png" alt="">
                <div>
                    <h3> ꙰    ☁ part n, the beginning</h3>

                    <p> i grew, i brought you my new life, i know where you are and hopefully will always be</p>
                    <p> i committed this so next time your warm hugs my face i can keep record of how much i love
                        to hate you</p>
                        <br>
                    <p> and how you've made me who i am, a little structured, a little choatic, sometimes warm,
                        unconventially beautiful, full of life, and only getting started </p>
                     <br>
            
                </div>
            </div>

        </section>

        <section class="white">
            <div class="row-left">

                <p> made to make me feel something </p>
                <br>
                <p> or nothing | by <a href="https://malgamves.dev"> daniel </a></p>

            </div>

        </section>





    </main>
</template>

<script setup lang="ts">

useHead({
    link: [
        {
            rel: 'preconnect',
            href: 'https://fonts.googleapis.com'
        },
        {
            rel: 'stylesheet',
            href: 'https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;0,400;0,500;1,300&display=swap',
            crossorigin: ''
        }
    ]
});
</script>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    data() {
        return {
            audio: HTMLAudioElement | null,
            timer: 0,
            isAutoplay: false,
        };
    },
    mounted() {
        this.audio = new Audio(
            'https://cdn.pixabay.com/download/audio/2022/06/13/audio_54f6c2ba71.mp3?filename=dark-sad-ambient-piano-113208.mp3'
            // 'https://www.dropbox.com/s/zt44wy6nryj0g6e/hearty%20sound-danny-docu.wav'
        );
    },
    methods: {
        async setAutoplay() {
            if (!this.audio) return;
            await this.audio.play(); // play() once now, you can directly call play() later.
            this.audio.pause();
            this.isAutoplay = true;
            this.timer = setInterval(() => {
                this.audio?.play();
            }, 3000);
        },
        stopAutoplay() {
            this.isAutoplay = false;
            clearInterval(this.timer);
        },
    },
});


</script>

<!-- <script setup>

var sound = 'https://cdn.pixabay.com/download/audio/2022/06/13/audio_54f6c2ba71.mp3?filename=dark-sad-ambient-piano-113208.mp3'
var audio = new Audio(sound);


const playSound = ({ target: { scrollTop, clientHeight, scrollHeight } }) => {
    console.log("scroll"); // I don't get "scroll" in console.

    audio.play();
    if (scrollTop + clientHeight >= scrollHeight) {
        console.log("bottom");
    }
}

</script> -->

<style>
/** Full Page Scroll-Snapping HTML Sections */
main {
    height: 100vh;
    overflow-y: auto;
    scroll-snap-type: y mandatory;
    font-family: 'Cormorant', serif;
    color: #FFFFFA;
}

section {
    height: 100vh;
    scroll-snap-align: center;
}

/** section colors */
.red {
    background: #f44336;
}

.white {
    background: white;
}

/** Section inner layout */
section {
    padding-left: 12em;
    padding-right: 12em;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

/** Reset / Basic styling */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    color: #fff;
    font-size: 1.6vmax;
}

h1 {
    font-size: 4em;
    color: black;
}

h3 {
    font-size: 1em;
    color: black;
    padding-bottom: 15px;
}

img {
    width: 400px;
    /*20%*/
    height: 400px;
    /*20%*/
    margin-right: 5%;
    margin-left: 5%;
    border-radius: 14px;

}

.row {
    display: flex;
    margin: 2%;
    /*justify-content: space-between;*/
}

.row-text {
    display: flex;
    margin: 2%;
    display: flex;
    /*justify-content: space-between;*/
}

.row-left {
    display: flex;
    margin: 2%;
    justify-content: space-between;
}

p {
    color: black;
}


.wrapper:hover .figure {
    transform: scale(0.9);
}

.wrapper:hover .img {
    transform: scale(1.111);
}


.wrapper {
    width: 400px;
}

.figure,
.img {
    will-change: transform;
    transition: transform .3s;
}

.figure {
    overflow: hidden;
}
</style> 

