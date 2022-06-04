<template>
	<div id="app">
		<headerVue />

		<aboutVue />

		<socialsVue />

		<contactVue />
	</div>
</template>

<script>
import headerVue from './header.vue';
import aboutVue from './about.vue';
import socialsVue from './socials.vue';
import contactVue from './contact.vue';

export default
{
	name: 'app',
	components: { headerVue, aboutVue, socialsVue, contactVue }
}
</script>

<style lang="scss">
*
{
    box-sizing: border-box;
}

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

fieldset
{
    width: fit-content;
    max-width: 90%;
    text-align: center;

    margin: 1em auto;
    padding: 1em 2em;
    
    color: var(--main-color);
    border: 1px solid var(--main-color);
    border-radius: 5px;
}

legend
{
    font-size: 1.75em;
}

fieldset p
{
    font-size: 1.25em;

    & a
    {
        color: inherit;
    }
}
</style>