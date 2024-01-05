<script>
    export let logo = "";
    export let name = "";
    export let description = "name";
    export let stack = "";
    export let width = "";
</script>

<div class="line"></div>

<div class="container">
    <img src={logo} alt="zonder" width={width}/>
    <h2>{name}</h2>
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
    h2 {
        font-size: 20px;
        margin-top: 20px;
    }

    .line {
        background: #2f2f2f;
        height: 1px;
    }

    .container {
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