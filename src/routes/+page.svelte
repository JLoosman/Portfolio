<script>
  import Point from "./Point.svelte";
</script>

<div class="text">
  <h1>Jesiah Loosman</h1>
</div>
<div class="overlay"></div>
<div class="grid">
  {#each Array(2000) as _, i}
    <Point />
  {/each}
</div>

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
    color: #eee;
    font-size: 120px;
    z-index: 1;
  }
</style>

