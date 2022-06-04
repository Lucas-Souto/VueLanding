<template>
    <div id="about">
        <p>
            VueLanding é uma aplicação de landing page simples para estudos com vue. <br />
            Desenvolvido por: <a href="https://github.com/Lucas-Souto" target="_blank">Lucas Souto</a>
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
    width: fit-content;
    font-size: 1.25em;
    text-align: center;

    margin: 1em auto;
    padding: .25em .5em;

    color: var(--main-color);
    border: 1px solid var(--main-color);
    border-radius: 5px;

    & a
    {
        color: inherit;
    }
}
</style>