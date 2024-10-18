<script>
  export let file;
  export let name;
  export let bio;
  export let images;
</script>

<div class="project-section">
  <h2>{name}</h2>
  <p>{bio}</p>
  <div class="collage">
    {#each { length: 3 } as _, i}
      <div class="column">
        {#each images as imageColumn}
          <img
            src="/individuals/{file}/{imageColumn[i]}"
            alt=""
          />
        {/each}
      </div>
    {/each}
  </div>
</div>

<style>
  h2 {
    padding-bottom: 10px;
    font-weight: 900;
    border-bottom: 2px solid #c72027;
    color: #c72027;
  }

  p {
    margin-bottom: 60px;
    font-weight: 700;
    padding-right: 20vw;
    color: #c72027;
    font-size: 22px;
  }

  img {
    max-width: 100%;
  }

  .collage {
    display: flex;
    flex-wrap: wrap;
  }

  .column {
    flex: 50;
    max-width: 50%;
    padding: 0 4px;
  }

  .column img {
    margin-top: 8px;
    vertical-align: middle;
    width: 100%;
  }

  @media only screen and (max-width: 1400px) {
    p {
      font-size: 18px;
    }
  }
</style>
