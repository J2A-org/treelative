<script>
  import Graph from '$lib/components/Graph.svelte'
</script>

<main>
  <h1>Treelative</h1>
  <p>🌲 Family Tree Visualization</p>
  <div class='playground'>
    <Graph />
  </div>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
  }
  h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  p {
    font-size: 1.5rem;
    margin-bottom: 1rem;
  }
  .playground {
    width: 400px;
    height: 400px;
    background-color: black;
    color: white;
    padding: 1rem;
  }
</style>