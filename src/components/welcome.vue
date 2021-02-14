<template>
	<div id="welcome">
		<div id="welcome-sentence-1">Hi! Welcome to</div>
		<div id="welcome-sentence-2">Sam Guo's Page</div>
		<div id="welcome-img">
			<img id="welcome-my-icon" src="../assets/img/Sam-Guo-Logo.png" alt="my-icon">
		</div>
	</div>
</template>

<script>
export default {
	el: '#welcome'
}
</script>

<style lang="scss">
:root {
	--title-ratio: calc(16 / 9);
	--title-font-size: 6vw;
	@media screen and (max-width: 990px) {
		--title-ratio: calc(3 / 3);
	}
}
</style>

<style lang="scss" scoped>
// use grid to construct the welcome body
#welcome {
	width: 100%;
	height: calc(1 / var(--title-ratio) * 100vw);

	display: grid;
	grid-template-columns: 1.4fr 1fr;
	grid-template-rows: 3fr 1fr 1fr 3fr;
	grid-template-areas: 
		". welcome-img"
		"welcome-sentence-1 welcome-img"
		"welcome-sentence-2 welcome-img"
		". welcome-img";
	
	&-sentence-1 {
		grid-area: welcome-sentence-1;
		place-self: center center;

		font-size: var(--title-font-size);
		font-family: font-curly;
		color: var(--welcome-color2);
	}

	&-sentence-2 {
		grid-area: welcome-sentence-2;
		place-self: center center;

		font-size: var(--title-font-size);
		font-family: font-curly;
		color: var(--welcome-color1);
	}

	&-img {
		grid-area: welcome-img;

		/* flex is more convenient with images */
		display: flex;
		justify-content: center;
		align-items: center;
		// background-color: #11EBCD;
	}

	&-my-icon {
		width: 60%;
		padding-right: 10%;
	}
}

#my-icon {
	width: 60%;
	padding-right: 10%;
}

// change the layout when the maximum width of the screen is smaller than 990px
@media screen and (max-width: 990px) {
	#welcome {
		width: 100%;
		height: calc(var(--title-ratio) * 100vw);
	
		grid-template-columns: 1fr 6fr 1fr;
		grid-template-rows: 10fr 1fr 1fr;
		grid-template-areas: 
			". welcome-img ."
			". welcome-sentence-1 ."
			". welcome-sentence-2 .";

		&-my-icon {
			width: 60%;
			padding-right: 0%;
		}
	}
}
</style>