<template>
    <fieldset id="about">
        <legend>About</legend>

        <p>
            VueLanding is a simple landing page application for studies with vue. <br />
            Developed by: <a href="https://github.com/Lucas-Souto" target="_blank">Lucas Souto</a>
        </p>
    </fieldset>
</template>

<script>
export default
{
    name: 'about'
}
</script>

<style lang="scss">
#about
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

#about legend
{
    font-size: 1.75em;
}

#about p
{
    font-size: 1.25em;

    & a
    {
        color: inherit;
    }
}
</style>