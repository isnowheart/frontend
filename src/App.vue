<template lang="pug">
	#app
		header-component
		menu-component
		div-component
		footer-component
</template>

<script>
import HeaderComponent from "@/components/layouts/Header"
import MenuComponent from "@/views/components/Menu"
import ContentComponent from "@/views/Content"
import FooterComponent from "@/components/layouts/Footer"

export default {
	name: "App",
	components: { HeaderComponent, MenuComponent, ContentComponent, FooterComponent }
}
</script>

<style scoped>
body {
	margin: 0;
}
	#app {
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;

		height: 100vh;
		display: grid;
		grid-template-rows: 60px 1fr 40px;
		grid-template-columns: 300px 1fr;
		grid-template-areas: 
			"header header" 
			"menu content" 
			"menu footer"; 
	}
</style>