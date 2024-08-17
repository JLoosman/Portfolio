<script>
  let size = Math.floor(Math.random() * 1.5) + 1;
</script>

<div class="box">
  <div class="block" style="--heightDot: {size}px; --widthDot: {size}px"></div>
</div>

<style>
  .box {
    height: 32px;
    width: 32px;
  }
  .block {
    margin: 15px;
    background-color: #eee;
    height: var(--heightDot);
    width: var(--widthDot);
    border-radius: 5px;
  }
</style>
