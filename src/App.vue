<template>
  <div id="app">
    <headrow></headrow>
  </div>
</template>

<script>
import headrow from './components/headrow.vue'

export default {
  name: 'App',
  components: {
    headrow
  }
}
</script>

<style>
/* font setting template */
@font-face {
	font-family: titlefont;
	src: url('./assets/font/Courgette-Regular.ttf');
}

/* global variables */
:root {
	--main-color1: #004edb;
	--main-color2: black;
	--title-ratio: calc(16 / 9);
	--title-font-size: 6vw;
	--headrow-height: 60px;
}

/* normalize setting */
html {
	line-height: 1.15;
	-webkit-text-size-adjust: 100%;
}

img {
	border-style: none;
}

body {
	margin: 0;
	padding: 0;
	background-color: white;
}
</style>
