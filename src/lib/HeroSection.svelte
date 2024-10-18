<section>
  <div class="wrapper">
    <img
      src="/tiles-logo.png"
      alt="Logo of NUNG Exhibition, featuring 4 aesthetic tiles patterns representing 4 disciplines of design found within the exhibition."
    />
    <div class="content">
      <h1>NUNG is RMIT's fieriest kiln!</h1>
      <h2>
        A Capstone 2 Exhibition, showcasing the works of RMIT University's Final Year Design
        Students, where the finest ceramics and tiles come to life!
      </h2>
    </div>
  </div>
</section>

<style>
  section {
    background-color: #c72027;
    height: 100vh;
    width: 100%;
  }

  .wrapper {
    margin: 0;
    padding: 0;
    width: 100%;
    height: auto;
    display: flex;
    justify-content: space-between;
    align-items: end;
  }

  .content {
    width: 45vw;
    margin: 0 30px;
    padding: 0;
  }

  img {
    width: 36.75vw;
    height: auto;
    max-height: 75vh;
    max-width: 75vh;
    margin-top: 120px;
    margin-left: 30px;
  }

  h1 {
    color: white;
    font-size: 40px;
    font-weight: 900;
  }

  h2 {
    color: white;
    font-size: 20px;
    font-weight: 500;
    margin: 0;
  }

  @media only screen and (orientation: portrait) {
    section {
      height: fit-content;
    }
  }

  @media only screen and (max-width: 1200px) {
    div {
      width: 100%;
    }

    h1 {
      font-size: 30px;
    }
  }

  @media only screen and (max-width: 992px) {
    section {
      padding-bottom: 40px;
    }

    h1 {
      font-size: 24px;
    }

    h2,
    p {
      font-size: 18px;
    }
  }

  @media only screen and (max-width: 576px) {
    .wrapper {
      display: block;
    }

    img {
      width: 84%;
      margin-right: auto;
      margin-bottom: 60px;
    }

    .content {
      width: 84%;
    }

    h1 {
      font-size: 22px;
    }
  }
</style>
