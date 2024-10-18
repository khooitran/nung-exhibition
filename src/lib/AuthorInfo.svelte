<script>
  export let name;
  export let bio;
  export let mail;
  export let website;
</script>

<div>
  <h2>{name}</h2>
  <p>{bio}</p>
  <a href="mailto:{mail}">Gmail &rarr;</a>
  <a href="{website}">Portfolio &rarr;</a>
</div>

<style>
  div {
    position: fixed;
    width: 25%;
    z-index: -1;
  }

  h2,
  p,
  a {
    color: #c72027;
  }

  p {
    font-weight: 700;
    font-size: 22px;
    margin-bottom: 60px;
  }

  h2 {
    font-weight: 900;
    padding-bottom: 10px;
    border-bottom: 2px solid #c72027;
  }

  a {
    font-size: 24px;
    text-decoration: none;
    font-weight: 900;
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

  @media only screen and (max-width: 768px) {
    div {
      position: static;
      width: 100%;
      margin-top: 40px;
    }
  }
</style>
