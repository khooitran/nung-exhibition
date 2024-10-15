<section>
  <div class="wrapper">
    <img
      src="/about/core-team.png"
      alt="The core team of NUNG Exhibition"
    />
    <div>
      <p>Core Team</p>
      <p>Trần Khánh Linh</p>
      <p>Nguyễn Phương Nhung</p>
      <p>Từ Bảo Ngân</p>
      <p>Nguyễn Thùy Trang</p>
      <p>Đinh Song Linh</p>
    </div>
  </div>

  <div class="wrapper">
    <img
      src="/about/operation-team.jpg"
      alt="The operation team of NUNG Exhibition"
    />
    <div>
      <p>Operation Team</p>
      <p>Nguyễn Thùy Trang</p>
      <p>Nguyễn Đặng Hùng Sơn</p>
      <p>Nguyễn Đoàn Minh Quân</p>
      <p>Đặng Quốc Anh</p>
    </div>
  </div>

  <div class="wrapper">
    <img
      src="/about/design-team.jpg"
      alt="The design team of NUNG Exhibition"
    />
    <div>
      <p>Design Team</p>
      <p>Đinh Song Linh</p>
      <p>Nguyễn Ngọc Quỳnh Hương</p>
      <p>Nguyễn Hoàng Long</p>
      <p>Nguyễn Đức Duy</p>
      <p>Nguyễn An Sơn</p>
      <p>Nguyễn Đỗ Quỳnh Anh</p>
      <p>Lê Hoàng Sơn</p>
    </div>
  </div>

  <div class="wrapper">
    <img
      src="/about/pr-team.jpg"
      alt="The public relations team of NUNG Exhibition"
    />
    <div>
      <p>PR Team</p>
      <p>Từ Bảo Ngân</p>
      <p>Đỗ Hạnh Mi</p>
      <p>Nguyễn Thu Hải</p>
      <p>Nguyễn Đỗ Quỳnh Anh</p>
      <p>Nguyễn Lê Thảo Nguyên</p>
    </div>
  </div>

  <div class="wrapper">
    <img
      src="/about/lecturers.jpeg"
      alt="The lecturers of Capstone 2 and also the managers of NUNG Exhibition"
    />
    <div>
      <p>Lecturers</p>
      <p>Jon Kuiter</p>
      <p>Colm Dunne</p>
    </div>
  </div>
</section>

<style>
  section {
    margin-top: 100px;
    margin-left: 30px;
  }

  .wrapper {
    display: flex;
    margin-bottom: 50px;
  }

  img {
    width: 50%;
    height: auto;
  }

  p {
    margin: 0 0 1px 30px;
    color: #c72027;
    font-weight: 900;
    font-size: 24px;
  }

  .wrapper p:nth-child(1) {
    width: 30vw;
    margin-bottom: 20px;
    font-style: normal;
    border-bottom: 2px solid #c72027;
  }

  @media only screen and (max-width: 1200px) {
    p {
      font-size: 18px;
    }
  }

  @media only screen and (max-width: 576px) {
    .wrapper {
      flex-direction: column;
      margin-right: 30px;
    }

    .wrapper div {
      margin-top: 15px;
    }

    img {
      width: 100%;
    }

    p {
      margin-left: 0;
    }

    .wrapper p:nth-child(1) {
      width: 100%;
    }
  }
</style>
