<template>
	<div id="app">
		<headerVue />
	</div>
</template>

<script>
import headerVue from './header.vue'

export default
{
	name: 'app',
	components: { headerVue }
}
</script>

<style lang="scss">
@import url('./assets/normalize.css');

#app
{
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
</style>