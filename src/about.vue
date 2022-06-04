<template>
    <div id="about">
        <h2>About</h2>

        <p>
            VueLanding is a simple landing page application for studies with vue. <br />
            Developeed by: <a href="https://github.com/Lucas-Souto" target="_blank">Lucas Souto</a>
        </p>
    </div>
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
    width: 90%;
    text-align: center;

    margin: 1em auto;
    
    color: var(--main-color);
}

#about p
{
    width: fit-content;
    font-size: 1.25em;

    margin: 1em auto;
    padding: .75em 1em;
    border: 1px solid var(--main-color);
    border-radius: 5px;

    & a
    {
        color: inherit;
    }
}
</style>