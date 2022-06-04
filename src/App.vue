<template>
	<div id="app">
		<headerVue />

		<aboutVue />
	</div>
</template>

<script>
import headerVue from './header.vue';
import aboutVue from './about.vue';

export default
{
	name: 'app',
	components: { headerVue, aboutVue }
}
</script>

<style lang="scss">
body
{
	background-color: #18222c;
}

#app
{
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
</style>