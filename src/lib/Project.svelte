<script>
    import { fade } from "svelte/transition";

    export let logo = "";
    export let name = "";
    export let description = "name";
    export let stack = "";
    export let width = "";
    export let link = "";

    let urlPopup = false;

    function toggleUrlPopup(){
        urlPopup = !urlPopup;
    }
</script>

<div class="line"></div>

<div class="container">
    <img src={logo} alt="zonder" width={width}/>
    <div class="ye">
        {#if urlPopup}
            <div class="url" transition:fade>
                {link}
            </div>
        {/if}
        <a class="title" href={link} target="_blank" on:mouseenter={() => toggleUrlPopup()} on:mouseleave={ () => toggleUrlPopup() }>{name}</a>
    </div>
    <p>
        {description}
    </p>

    <div class="stack">
        <img src="/logos/stack.svg" alt="stack" width="24px"/>
        <p>{stack}</p>
    </div>
</div>

<div class="line"></div>

<style>
    .ye {
        margin-top: 20px;
    }

    .url {
        position: absolute;
        border-radius: 8px;
        top: 70px;
        background: rgba(0, 0, 0, 0.5);
        padding: 6px 8px;
        left: -30px;
    }
    
    .title {
        font-size: 20px;
        font-weight: 600;
    }

    .line {
        background: #2f2f2f;
        height: 1px;
    }

    .container {
        position: relative;
        display: flex;
        flex-direction: column;
        gap: 10px;
        padding: 14px 0;
    }

    .stack {
        display: flex;
        align-items: center;
        gap: 12px;
        margin-top: 16px;
    }

    .stack p {
        font-size: 14px;
    }

    .container p {
        line-height: 23px;
        font-size: 15px;
    }
</style>