<template>
  <div id="app">
    <headrow/>
	<welcome/>
  </div>
</template>

<script>
import headrow from './components/headrow.vue'
import welcome from './components/welcome.vue'

export default {
  name: 'App',
  components: {
    headrow,
	welcome
  }
}
</script>

<style>
/* font setting template */
@font-face {
	font-family: font-curly;
	src: url('./assets/font/Courgette-Regular.ttf');
}

/* global variables */
:root {
	--transition-width: '990px';
	--welcome-color1: #004edb;
	--welcome-color2: black;
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
