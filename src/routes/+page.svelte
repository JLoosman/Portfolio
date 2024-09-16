<script>
  import typer from "typer-js";
  import { onMount } from "svelte";
  import Point from "./Point.svelte";
  import { reveal } from "svelte-reveal";

  let revealConfig = {
    preset: "slide",
    y: 40,
    x: 0,
    opacity: 0,
    duration: 600,
    blur: 0,
  };

  onMount(() => {
    typer(".text h1", { min: 20, max: 350 }).line("Jesiah Loosman");
  });
</script>

<div class="text">
  <h1></h1>
</div>
<div class="overlay"></div>
<div class="grid">
  {#each Array(1500) as _}
    <Point />
  {/each}
</div>

<section>
  <h2 use:reveal={revealConfig}>Projekte</h2>
  <a use:reveal={revealConfig} href="/projekte">Hier klicken!</a>
</section>
<section class="left">
  <h2 use:reveal={revealConfig}>Skills</h2>
  <a use:reveal={revealConfig} href="/skills">Hier klicken!</a>
</section>
<section>
  <h2 use:reveal={revealConfig}>Kontakt</h2>
  <a use:reveal={revealConfig} href="/kontakt">Hier klicken!</a>
</section>

<style>
  .grid {
    height: 100%;
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    overflow: hidden;
    background-color: #000;
  }

  .overlay {
    height: 100vh;
    width: 100vw;
    position: absolute;
    top: 0;
    left: 0;
    background-image: radial-gradient(#ffffff00, #000000 95%);
  }

  .text {
    height: 100vh;
    width: 100vw;
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .text h1 {
    user-select: none;
    color: #eee;
    font-size: 100px;
    font-family: Aldrich, sans-serif;
    z-index: 1;
    text-align: center;
  }

  section {
    padding: 20px 20%;
    height: 60%;
    width: 100%;
    background-color: #000;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: end;
  }

  section h2 {
    color: #eee;
    font-size: 60px;
    margin-bottom: 20px;
  }

  section a {
    text-decoration: none;
    color: #111;
    background-color: #eee;
    padding: 10px 20px;
    border-radius: 10px;
  }

  section a:hover {
    color: #eee;
    background-color: #999;
  }

  .left {
    align-items: start;
  }
</style>
