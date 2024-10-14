<script>
  export let file;
  export let name;
  export let author;
</script>

<a href="/projects/{file}">
  <img
    src="/thumbnails/{file}.png"
    alt="{name}"
  />
  <p>{name}<br />{author}</p>
</a>

<style>
  img {
    width: 100%;
    margin-top: 30px;
  }

  a {
    text-decoration: none;
    color: #c72027;
    font-weight: 900;
  }

  a:hover {
    text-decoration: underline;
  }

  p {
    margin-top: 10px;
  }
</style>
