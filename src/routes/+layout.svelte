<script>
    import '../app.css';
    import Header from '$lib/Header.svelte';
    import Footer from "$lib/Footer.svelte";
</script>

<style>
    :root {
        --accent: #67a5e8;
    }
</style>

<div class="background"></div>
<Header />
<slot />
<Footer />