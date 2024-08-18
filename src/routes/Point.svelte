<script>
  let size = Math.floor(Math.random() * 1.5) + 1;
  let animationTime = Math.random() * 5 + 4;

  setInterval(() => {
    size = Math.floor(Math.random() * 1.5) + 1;
  }, 1000000);
</script>

<div class="box">
  <div
    class="block"
    style="--heightDot: {size}px; --widthDot: {size}px; --time: {animationTime}s;"
  ></div>
</div>

<style>
  .box {
    height: 38px;
    width: 38px;
  }
  .block {
    margin: 15px;
    background: rgba(255, 255, 255, 0);
    height: var(--heightDot);
    width: var(--widthDot);
    border-radius: 5px;
    animation: twinkle var(--time) linear var(--time) infinite;
  }

  @keyframes twinkle {
    0% {
      transform: scale(1, 1);
      background: rgba(255, 255, 255, 0);
      animation-timing-function: ease-in;
    }
    20% {
      transform: scale(0.8, 0.8);
      background: rgba(255, 255, 255, 1);
      animation-timing-function: ease-out;
    }
    40% {
      background: rgba(255, 255, 255, 0);
      transform: scale(1, 1);
    }
    100% {
      background: rgba(255, 255, 255, 0);
      transform: scale(1, 1);
    }
  }
</style>
