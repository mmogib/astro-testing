<script context="module">
</script>

<script lang="ts">
  let counter: number = 0;

  const addOne = (count: number): number => {
    return count + 1;
  };

  const subtract = (count: number): number => {
    return count - 1;
  };
</script>

<div id="svelte" class="counter">
  <button on:click={() => (counter = subtract(counter))}>-</button>
  <pre>{counter}</pre>
  <button on:click={() => (counter = addOne(counter))}>+</button>
</div>
