<script>
  import typer from "typer-js";
  import { onMount } from "svelte";
  import Point from "./Point.svelte";

  onMount(() => {
    typer(".text h1", { min: 20, max: 350 }).line("Jesiah Loosman");
  });
</script>

<div class="text">
  <h1></h1>
</div>
<div class="overlay"></div>
<div class="grid">
  {#each Array(1500) as _, i}
    <Point />
  {/each}
</div>

<section>
  <p>
    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Libero praesentium
    rerum deserunt vero ducimus alias animi, iste totam esse similique.
    Quibusdam eligendi incidunt placeat eum libero ab voluptatibus, quas non.
  </p>
</section>

<style>
  .grid {
    height: 100%;
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    overflow: hidden;
    background-color: #000;
    /* could also be #111, gives kind of spotlight effect*/
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
  }
</style>
