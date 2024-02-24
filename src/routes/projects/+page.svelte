<script>
    import Projects from "$lib/Projects.svelte";
</script>

<div class="container">
    <Projects />
</div>

<style>
    .container {
        display: flex;
        align-items: center;
        margin: 0 auto;
        max-width: 900px;
    }

    @media screen and (max-width: 768px){
        .container {
            width: 80vw;
        }
    }
</style>