<template>
    <main >

        <section class="white">
            <div>
                <img ref="img" src="https://i.imgur.com/MLDDpTV.png" alt="">
                <div>
                    <h3> ꙰    ☁ part 1, the end</h3>
                    <p id="drag"> wild heards beat for the plains that nurtered them, til the thing that kept them alive stops
                        their breathings.</p>
                    <br>
                    <p id="drag">it hurts to leave but will i ever know anything outside your sheltered streets and tiny store</p>
                    <br>
                    
                    <hr>

                </div>
            </div>

        </section>



        <section class="white">
            <div class="row">
                <div>
                    <h3> ꙰    ☁ part 2, the fire</h3>
                    <p id="drag"> it hurts to leave but i do because when i hear melissa i think about thier bread, i heard they
                        burned down and i waasn't there to talk about how tragic it might be to stay stuck when i could
                        swim in the oceans</p>
                        <br>
                    <p id="drag"> it hurt to leave but i had to grow, the one thing that didn't thrive in that mild savanna was my
                        will to live.</p>
                    <br>
                    

                </div>
                <img id="drag" src="https://i.imgur.com/3PJtQ93.png" alt="">
            </div>
        </section>

    </main>
</template>

<script setup>

import { ref, onMounted } from 'vue'

// declare a ref to hold the element reference
// the name must match template ref value
const img = ref(null)

onMounted(() => {
  img.value.focus()
})

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

<script>

dragElement(document.getElementById("mydiv"));

function dragElement(elmnt) {
  var pos1 = 0, pos2 = 0, pos3 = 0, pos4 = 0;
  if (document.getElementById(elmnt.id + "header")) {
    // if present, the header is where you move the DIV from:
    document.getElementById(elmnt.id + "header").onmousedown = dragMouseDown;
  } else {
    // otherwise, move the DIV from anywhere inside the DIV:
    elmnt.onmousedown = dragMouseDown;
  }

  function dragMouseDown(e) {
    e = e || window.event;
    e.preventDefault();
    // get the mouse cursor position at startup:
    pos3 = e.clientX;
    pos4 = e.clientY;
    document.onmouseup = closeDragElement;
    // call a function whenever the cursor moves:
    document.onmousemove = elementDrag;
  }

  function elementDrag(e) {
    e = e || window.event;
    e.preventDefault();
    // calculate the new cursor position:
    pos1 = pos3 - e.clientX;
    pos2 = pos4 - e.clientY;
    pos3 = e.clientX;
    pos4 = e.clientY;
    // set the element's new position:
    elmnt.style.top = (elmnt.offsetTop - pos2) + "px";
    elmnt.style.left = (elmnt.offsetLeft - pos1) + "px";
  }

  function closeDragElement() {
    // stop moving when mouse button is released:
    document.onmouseup = null;
    document.onmousemove = null;
  }
}

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

/** styling for dragging element **/
#drag {
    position: absolute;
    z-index: 9;
    background-color: #f1f1f1;
    border: 1px solid #d3d3d3;
    text-align: center;
    cursor: move;
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

<!-- reference on dragging components 
    https://markus.oberlehner.net/blog/refs-and-the-vue-3-composition-api/
    https://www.w3schools.com/howto/howto_js_draggable.asp -->