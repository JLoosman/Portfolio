<script>
  import "../app.css";
</script>

<a href="/" class="home">
  <svg
    width="50"
    height="50"
    viewBox="0 0 50 50"
    style="color:currentColor"
    xmlns="http://www.w3.org/2000/svg"
    class="h-full w-full"
    ><rect
      width="50"
      height="50"
      x="0"
      y="0"
      rx="30"
      fill="transparent"
      stroke="transparent"
      stroke-width="0"
      stroke-opacity="100%"
      paint-order="stroke"
    ></rect><svg
      width="50px"
      height="50px"
      viewBox="0 0 24 24"
      fill="currentColor"
      x="0"
      y="0"
      role="img"
      style="display:inline-block;vertical-align:middle"
      xmlns="http://www.w3.org/2000/svg"
      ><g fill="currentColor"
        ><path
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M21 19v-6.733a4 4 0 0 0-1.245-2.9L13.378 3.31a2 2 0 0 0-2.755 0L4.245 9.367A4 4 0 0 0 3 12.267V19a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2Z"
        /></g
      ></svg
    ></svg
  >
</a>
<main>
  <slot />
</main>

<style>
  main {
    height: 100vh;
    width: 100vw;
    background-color: #000;
  }

  .home {
    position: fixed;
    top: 50px;
    left: 50px;
    color: #fff;
    z-index: 2;
  }
</style>
