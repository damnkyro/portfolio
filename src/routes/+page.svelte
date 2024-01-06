<script>
  import Commissions from "$lib/Commissions.svelte";
  import Contact from "$lib/Contact.svelte";
  import Hero from "$lib/Hero.svelte";
  import Projects from "$lib/Projects.svelte";
  import Skills from "$lib/Skills.svelte";
</script>

<div class="container">
  <div>
    <Hero />
    <Skills />
    <Projects />
    <p id="more-projects">
      You can find more of my projects <a href="/projects" class="project-link"
        >here</a
      >
      or on
      <a class="project-link" target="_blank" href="https://github.com/damnkyro">github</a>
    </p>
    <Commissions />
    <Contact />
  </div>
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 10px auto;
    width: 50vw;
  }

  .project-link {
    color: var(--accent);
  }

  #more-projects {
    line-height: 22px;
    margin-top: 20px;
  }

  @media screen and (max-width: 768px) {
    .container {
      width: 80vw;
    }
  }
</style>
