<script>
  import Card from "./Card.svelte";
  export let posts = [];
</script>

<section class="TimeLine">
  <article class="TimeLine-container">
    {#each posts as post}
      <Card {...post} />
    {:else}
      <p>Loading...</p>
    {/each}
  </article>
</section>

<style>
  .TimeLine {
    padding: 4em 0 0 0;
  }
</style>
