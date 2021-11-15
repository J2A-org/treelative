<script>
  import { onMount } from 'svelte'

  onMount(() => {
    handleResize()
  })

  const handleResize = () => {
    // fix for 100vh height for mobile: use with calc(100 * var(--vh))
    document.querySelector(':root').style.setProperty('--vh', window.innerHeight / 100 + 'px')
  }
</script>

<svelte:window on:resize={handleResize} />

<slot></slot>

<style>
  :global(body) {
    height: calc(100 * var(--vh));
    font-family: 'Roboto', sans-serif;
  }
  :global(#svelte) {
    height: 100%;
  }
</style>