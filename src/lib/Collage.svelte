<script>
  export let images;
  export let file;
  export let name;
</script>

<div class="collage">
  {#each { length: images.length } as _, i}
    <div class="column">
      {#each images as imageColumn}
        <img
          src="/individuals/{file}/{imageColumn[i]}"
          alt="{name}"
        />
      {/each}
    </div>
  {/each}
</div>

<style>
  img {
    max-width: 100%;
  }

  .collage {
    display: flex;
    flex-wrap: wrap;
  }

  .column {
    flex: 30%;
    max-width: 50%;
    padding: 0 4px;
  }

  .column img {
    margin-top: 8px;
    vertical-align: middle;
    width: 100%;
  }

  @media only screen and (max-width: 576px) {
    .column {
      flex: 100%;
      max-width: 100%;
    }
  }
</style>
