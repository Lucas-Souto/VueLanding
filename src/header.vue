<template>
    <header>
        <a class="header-group" href="/">
            <img id="header-logo" src="/src/assets/logo.png" />

            <h1 id="header-title">{{ title }}</h1>
        </a>
        
        <div id="header-options" class="header-group">
            <ul id="header-list">
                <li><a href='#about'>About</a></li>
                <li><a href='#socials'>Socials</a></li>
                <li><a href='#contact'>Contact</a></li>
            </ul>
        </div>
    </header>
</template>

<script>
export default
{
    name: 'headerVue',
    data()
    {
        return { title: 'V-Landing' }
    }
}
</script>

<style lang="scss">
header
{
    display: flex;
    justify-content: space-between;

    padding: .5em 1em;

    color: var(--main-color);
    background-color: var(--main-background-color);

    & a
    {
        text-decoration: none;

        color: inherit;
    }
}

.header-group
{
    display: flex;
    align-items: center;
}

#header-logo
{
    width: 4.5em;
    height: 4.5em;
}

#header-title
{
    margin: 0;
    margin-left: .5em;
}

#header-list
{
    list-style-type: none;

    padding: 0;
}

#header-list li
{
    float: left;
    font-size: 1.25em;

    border-radius: 2px;
    transition: .15s linear;

    & a
    {
        display: block;

        padding: .25em .5em;
    }

    &:hover
    {
        background-color: var(--main-dark-background-color);
    }
}

@media (max-width: 550px)
{
    header
    {
        align-items: center;
        flex-direction: column;
    }

    #header-options
    {
        width: 100%;
    }

    #header-list
    {
        width: inherit;
        display: flex;
        justify-content: space-evenly;

        & li
        {
            font-size: 1.4em;
        }
    }
}
</style>