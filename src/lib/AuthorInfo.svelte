<script>
  export let name;
  export let bio;
  export let mail;
  export let website = null;
  export let behance = null;
  export let instagram = null;
</script>

<div>
  <h2>{name}</h2>
  <p class="bio">{bio}</p>
  <a href="mailto:{mail}">Email &rarr;</a>
  {#if website}
    <a
      target="_blank"
      href="{website}">Portfolio &rarr;</a
    >
  {/if}
  {#if behance}
    <a
      target="_blank"
      href="{behance}">Behance &rarr;</a
    >
  {/if}
  {#if instagram}
    <a
      target="_blank"
      href="https://www.instagram.com/{instagram}">Instagram &rarr;</a
    >
  {/if}
</div>

<style>
  div {
    position: fixed;
    width: 25%;
  }

  h2,
  p,
  a {
    color: #c72027;
  }

  p {
    font-weight: 700;
    font-size: 22px;
    margin: 0;
  }

  .bio {
    margin-bottom: 60px;
  }

  h2 {
    font-weight: 900;
    padding-bottom: 10px;
    border-bottom: 2px solid #c72027;
  }

  a {
    font-size: 22px;
    text-decoration: none;
    font-weight: 700;
    display: block;
  }

  a:hover {
    text-decoration: underline;
  }

  @media only screen and (max-width: 1400px) {
    p,
    a {
      font-size: 18px;
    }
  }

  @media only screen and (max-width: 992px) {
    div {
      position: static;
      width: 100%;
      margin-top: 40px;
    }

    .bio {
      padding-right: 20vw;
    }
  }

  @media only screen and (max-width: 576px) {
    .bio {
      padding-right: 0;
    }
  }
</style>
