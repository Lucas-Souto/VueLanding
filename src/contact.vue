<template>
    <fieldset id="contact">
        <legend>Contact</legend>

        <h2 id="contact-message">
            Hello! I'm Lucas and I'll help you make any website that you can imagine. <br />
            Your creativity has no limits!
        </h2>

        <div class="separator"></div>

        <fieldset id="mail-area">
            <legend>Send E-Mail</legend>

            <fieldset class="input-legend">
                <input type="text" id="subject" placeholder="I want a site" />

                <legend>
                    <label for="subject">Subject</label>
                </legend>
            </fieldset>

            <fieldset class="input-legend">
                <input type="text" id="from" placeholder="fulano@gmail.com" />

                <legend>
                    <label for="from">From</label>
                </legend>
            </fieldset>

            <fieldset class="input-legend">
                <textarea type="text" id="message" placeholder="I'm fulano and I want..."></textarea>

                <legend>
                    <label for="message">Message</label>
                </legend>
            </fieldset>

            <button id="mail-send">Send</button>
        </fieldset>
    </fieldset>
</template>

<script>
export default { name: 'contact' }
</script>

<style lang="scss">
#contact
{
    width: 90%;
    display: flex;
    justify-content: space-between;
}

.separator
{
    height: auto;

    margin: 0 1em;

    border: 1px solid var(--main-color);
}

#contact-message
{
    font-size: 1.25em;
    align-self: center;
}

#mail-area
{
    width: 100%;
    margin: 0 auto;
}

.input-legend
{
    width: 100%;
    font-size: 1.25em;
    text-align: left;

    margin-bottom: 1em;
    padding: 0;

    & legend
    {
        font-size: 1em;

        margin-left: .5em;
    }

    & input,
    & textarea
    {
        width: 100%;
        resize: vertical;
        outline: none;

        padding: .25em .5em;

        color: var(--main-color);
        border: none;
        background-color: transparent;
    }
}

#mail-send
{
    cursor: pointer;
    width: 100%;
    font-size: 2em;

    padding: .25em .5em;

    color: var(--main-color);
    border: 1px solid var(--main-color);
    border-radius: 5px;
    background-color: var(--main-dark-background-color);
}

@media (max-width: 900px)
{
    #contact
    {
        flex-direction: column;
    }

    .separator
    {
        margin: 1em 0;
    }
}

@media (max-width: 380px)
{
    #contact
    {
        padding: .5em 1em;
    }

    #mail-area
    {
        padding: .25em;
    }
}
</style>