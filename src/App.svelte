<script>
  import Header from "./components/Header.svelte";
  import ProjectCard from "./components/ProjectCard.svelte";
  import Projects from "./components/Projects.svelte";

</script>

<main style="position: relative">
  <Header/>
  <hr>
  <Projects/>
  <ProjectCard projectTitle="Project Title" projectDescription="Project description llalalalalal alalalal alalalal alalala"/>
  <img src="assets\wipsign.gif" alt="Work in progress" width="128" height="128" id="wip-sign"/>
</main>

<style>
   /* Make sure the main element takes up the full height of the page */
   main {
    height: 100%;
  }

  hr {
        height: 100px;
        width: 90%;
    }

  #wip-sign {
    image-rendering: pixelated;
    display: block;
    margin: auto;
    padding-top: 200px;
  }
</style>
