<template>
    <fieldset id="socials">
        <legend>Socials</legend>

        <a class="social-icon" href="https://www.youtube.com/channel/UC_nVEXSIB-xQpVveQFXnM2Q" target="_blank">
            <img src="./assets/socials/youtube.svg" />
            <p class="social-tooltip">Youtube</p>
        </a>

        <a class="social-icon" href="https://www.instagram.com/lucas_souto15/" target="_blank">
            <img src="./assets/socials/instagram.svg" />
            <p class="social-tooltip">Instagram</p>
        </a>

        <a class="social-icon" href="https://twitter.com/OMathDev" target="_blank">
            <img src="./assets/socials/twitter.svg" />
            <p class="social-tooltip">Twitter</p>
        </a>
    </fieldset>
</template>

<script>
export default
{
    name: 'socials'
}
</script>

<style lang="scss">
#socials
{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
}

.social-icon
{
    box-sizing: unset;
    display: block;
    position: relative;
    width: 3em;
    height: 3em;

    margin: .5em;
    padding: 1em;

    border: 1px solid var(--main-color);
    border-radius: 5px;

    & img
    {
        width: 100%;
        height: 100%;
    }
}

.social-tooltip
{
    position: absolute;
    bottom: 95%;
    left: 50%;

    margin: 0;
    padding: .25em .5em;

    color: var(--main-dark-background-color);
    opacity: 0;
    border-radius: 10px;
    background-color: var(--main-color);
    transform: translate(-50%, -50%);
    transition: .25s ease-in-out;

    &::before
    {
        content: '';
        width: .5em;
        height: .5em;
        position: absolute;
        top: 100%;
        left: 50%;
        
        background-color: inherit;

        transform: translate(-50%, -50%) rotate(45deg);
    }
}

.social-icon:hover
{
    & .social-tooltip
    {
        opacity: 1;
    }
}
</style>