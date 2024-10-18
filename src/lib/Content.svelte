<script>
  export let name;
  export let bio;
</script>

<h2>{name}</h2>
<p>{bio}</p>

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

  @media only screen and (max-width: 1400px) {
    p {
      font-size: 18px;
    }
  }

  @media only screen and (max-width: 576px) {
    p {
      padding-right: 0;
    }
  }
</style>
