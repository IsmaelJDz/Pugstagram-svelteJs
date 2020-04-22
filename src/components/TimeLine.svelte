<script>

  import Card from "./Card.svelte"
  export let posts = [];

</script>

<!-- TimeLine.svelte -->

<style>
  .TimeLine {
    padding: 4em 0 0 0;
  }

  @media screen and (max-width: 1000px) {
    .TimeLine {
      padding: 0 4em 0 4em;
      grid-area: TimeLine
    }
  } 

</style>


<div class="TimeLine">
  <div class="TimeLine-container">
    {#each posts as post}
        <Card {...post} />
    {:else}
      <p>Loading...</p>
    {/each}
  </div>
</div>