<footer>
  <p class="title">NUNG Exhibition</p>
  <div class="flex">
    <div>
      <p>NUNG Exhibition Committee</p>
      <p>Bachelor of Design Studies</p>
      <p>School of Communication & Design</p>
      <p>from RMIT University Hanoi</p>
    </div>
    <div>
      <a
        target="_blank"
        href="https://www.instagram.com/nung.exhibition/">Instagram &rarr;</a
      >
      <a
        target="_blank"
        href="https://www.facebook.com/NUNG.exhibition">Facebook &rarr;</a
      >
    </div>
  </div>
</footer>

<style>
  footer {
    background-color: #c72027;
    padding: 36px 30px 50px;
    z-index: 1;
  }

  .flex {
    display: flex;
  }

  footer div div {
    margin-right: 100px;
  }

  p {
    margin: 0;
    padding: 0;
    color: #fffafa;
    font-size: 24px;
    font-style: italic;
  }

  .title {
    font-weight: 900;
    margin-bottom: 20px;
    font-style: normal;
  }

  a {
    color: #fffafa;
    text-decoration: none;
    font-size: 24px;
    font-style: italic;
    display: block;
  }

  a:hover {
    text-decoration: underline;
  }

  @media only screen and (max-width: 992px) {
    p,
    a {
      font-size: 16px;
    }
  }

  @media only screen and (max-width: 576px) {
    .flex div {
      margin-right: 10px;
      margin-bottom: 26px;
    }

    .flex {
      flex-direction: column;
    }

    footer {
      padding-bottom: 10px;
    }
  }
</style>
