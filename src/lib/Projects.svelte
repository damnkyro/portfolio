<script>
    import Project from "./Project.svelte";
</script>

<section>
    <div class="container">
       <div>
            <h2>Projects</h2>
            <p>These are a couple of projects that I have worked on for individuals / companies.</p>
            <Project
                name = "Hone"
                logo = "/media/hone.png"
                width = "55px"
                description = "Hone.lol is a biolink service that I made (similar to linktree)"
                stack = "Sveltekit, Supabase, Typescript"
                link="https://hone.lol"
            />

            <Project
                name = "Zonder"
                logo = "/media/zond.png"
                width = "80px"
                description = "Zonder is a streetwear brand. I designed a website for it writing the code for their frontend design and the server-side 
                logic for its payment gateway connected to the stripe API using sveltekit."
                stack = "Sveltekit, Typescript"
                link="https://thezonder.com"
            />

            <Project
                name = "Portfolio Site"
                logo = "/media/zen.jpg"
                width = "55px"
                description = "This is the website you are viewing right now!"
                stack = "Sveltekit, Typescript"
                link="https://kyro.lol"
            />
       </div>
    </div>
</section>

<style>
    h2 {
        font-size: 22px;
        font-weight: 700;
    }

    .container {
        display: flex;
        flex-direction: column;
        margin-top: 60px;
    }

    .container p {
        margin: 12px 0 24px 0;
        line-height: 22px;
    }
</style>