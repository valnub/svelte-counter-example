<script>
  let value = 0;
  export let max = 3;

  function increment() {
    if (value < max) value++;
  }

  function decrement() {
    if (value > 0) value--;
  }
</script>

<style>
  .counter > * {
    display: inline-block;
  }
</style>

<div class="counter">
  <button on:click={decrement}>-</button>
    <div>{value}</div>
  <button on:click={increment}>+</button>
</div>