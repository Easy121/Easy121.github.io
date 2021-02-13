<template>
	<div id="headrow">
		<div id="headrow-menu">
			<img id="headrow-menu-icon" src="../assets/img/menu-icon.png" alt="menu-icon">
		</div>
		<div id="headrow-explore">Explore</div>
		<div id="headrow-search">
			<img id="headrow-search-icon" src="../assets/img/search-icon.png" alt="search-icon">
		</div>
		<div id="headrow-transition"></div>
	</div>
</template>

<script>
export default {
	el: '#headrow'
}
</script>

<style lang="scss" scoped>
// use grid to construct headrow
#headrow {
	width: 100%;
	height: var(--headrow-height);

	display: grid;
	grid-template-columns: 1fr 9fr 3fr 1fr;
	grid-template-rows: 5fr 1fr;
	grid-template-areas: 
		"headrow-menu . headrow-explore headrow-search"
		"headrow-transition headrow-transition headrow-transition headrow-transition";

	&-menu {
		grid-area: headrow-menu;
		/* background-color: #11EBCD; */

		/* flex is more convenient with images */
		display: flex;
		justify-content: center;
		align-items: center;

		&-icon {
			width: calc(var(--headrow-height) - 30px);
		}
	}

	&-explore {
		grid-area: headrow-explore;
		/* background-color: #11EBCD; */

		font-family: titlefont;
		font-size: calc(var(--headrow-height) - 30px);

		place-self: center center;
	}

	&-search {
		grid-area: headrow-search;
		/* background-color: #11EBCD; */

		/* flex is more convenient with images */
		display: flex;
		justify-content: center;
		align-items: center;

		&-icon {
			width: calc(var(--headrow-height) - 35px);
		}
	}

	&-transition {
		grid-area: headrow-transition;
		background: 
			linear-gradient(black, grey 20%, white 80%);
		/* background-color: #11EBCD; */
	}
}
</style>

