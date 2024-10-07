<section>
  <img
    src="/tiles-logo.png"
    alt="Logo of NUNG Exhibition, featuring 4 aesthetic tiles patterns representing 4 disciplines of design found within the exhibition."
  />
  <div>
    <h2>
      “Nung” is a Capstone 2 Exhibition, showcasing the works of RMIT University’ Final Year Design
      Students. The concept of the project revolves around the imagery of different types of brick
      tile and the process of making bricks. The clay has to be molded, transformed, and fired
      (nung) under great heat in order to become a finished brick, which is a metaphor for design
      students undergoing many hardships before submitting their final works, showing themselves to
      the world.
    </h2>
    <p>
      The website is currently in production. Still, feel free to roam about the website and see it
      grow each day. Be aware of bugs and irregularities in this stage.
    </p>
  </div>
</section>

<style>
  section {
    background-color: #c72027;
    min-height: 100vh;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: start;
  }

  div {
    width: 40vw;
    margin: 115px 30px 20px 30px;
    padding: 0;
  }

  img {
    width: 36%;
    height: auto;
    max-height: 75vh;
    max-width: 75vh;
    margin-top: 120px;
    margin-left: 30px;
  }

  h2 {
    color: white;
    font-size: 24px;
    margin: 0;
  }

  p {
    color: white;
    font-size: 24px;
    font-style: italic;
    font-weight: 200;
  }

  @media only screen and (max-width: 1200px) {
    div {
      width: 100%;
    }
  }
  @media only screen and (max-width: 992px) {
    section {
      min-height: fit-content;
      padding-bottom: 40px;
    }
    h2,
    p {
      font-size: 18px;
    }
  }
  @media only screen and (max-width: 576px) {
    img {
      display: none;
    }
  }
</style>
