<template>
    <main>
	<section class="red">
		<h1>Red</h1>
		<h3>Excitement. Energy. Passion.</h3>
	</section>

    <section class="white">
        <div class="row">
  <img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg" alt="">
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
</div>

    </section>

	<section class="orange">
		<h1>Orange</h1>
		<h3> Energy. Balance. Enthusiasm.</h3>
	</section>

    <section class="white">
        <div class="row">
  
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
  <img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg" alt="">
</div>

    </section>

	<section class="yellow">
		<h1>Yellow</h1>
		<h3>Joy. Happiness. Sunshine.</h3>
	</section>

    <section class="white">
        <div class="wrapper">
  <figure class="figure">
    <img class="img" src="https://images.unsplash.com/photo-1667827002414-ebb2394a8674?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwzMjM4NDZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE2Njc5OTQ1Nzc&ixlib=rb-4.0.3&q=80" alt="Car in desert">
  </figure>
</div>
    </section>


	<section class="green">
		<h1>Green</h1>
		<h3>Nature. Environment. Healthy.</h3>
	</section>

	<section class="white">
        <div class="row">
  <img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg" alt="">
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
</div>

    </section>

	<section class="white">
        <div class="row">
  
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
  <img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg" alt="">
</div>

    </section>

	<section class="blue">
		<h1>Blue</h1>
		<h3>Peace. Tranquility. Calm.</h3>
	</section>

	<section class="indigo">
		<h1>Indigo</h1>
		<h3>Integrity. Knowledge. Power.</h3>
	</section>

	<section class="violet">
		<h1>Violet</h1>
		<h3>Royalty. Nobility. Spirituality.</h3>
	</section>

	<section class="white">
        <div class="row">
  <img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg" alt="">
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
</div>

    </section>


    
</main>
</template>

<style>
    /** Full Page Scroll-Snapping HTML Sections */
main {
	height: 100vh;
	overflow-y: auto;
	scroll-snap-type: y mandatory;
}

section {
	height: 100vh;
	scroll-snap-align: center;
}

/** section colors */
.red {
	background: #f44336;
}
.orange {
	background: #ff9800;
}
.yellow {
	background: #ffd600;
}
.green {
	background: #4caf50;
}
.blue {
	background: #2196f3;
}
.indigo {
	background: #3f51b5;
}
.violet {
	background: #673ab7;
}
.white {
    background: white;
}

/** Section inner layout */
section {
	padding-left: 4em;
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
	font-size: 2vmax;
}

h1 {
	font-size: 4em;
}

img {
  width: 400px; /*20%*/
  height: 400px; /*20%*/
  margin-right: 2%;
  margin-left: 2%;
}

.row {
  display: flex;
  margin: 2%;
  /*justify-content: space-between;*/
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

.figure, .img {
  will-change: transform;
  transition: transform .3s;
}

.figure {
  overflow: hidden;
}


</style> 

