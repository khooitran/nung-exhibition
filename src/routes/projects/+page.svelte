<script>
  let projects = [
    {
      file: 'adopt-to-adore',
      name: 'Adopt to Adore',
      author: 'Nguyễn Thu Hải',
    },
    {
      file: 'algorithmic-beauty',
      name: 'Algorithmic Beauty',
      author: 'Từ Bảo Ngân',
    },
    {
      file: 'bach-khoa-khong-toan-thu',
      name: 'Bách Khoa Không Toàn Thư',
      author: 'Trần Khánh Linh',
    },
    {
      file: 'changes',
      name: 'Changes - Perspectives on an Evolving City',
      author: 'Nguyễn Đặng Hùng Sơn',
    },
    {
      file: 'culture-archive',
      name: 'Cultural Archive: Ethnicities',
      author: 'Đinh Song Linh',
    },
    {
      file: 'dieu-phuc',
      name: 'Diệu Phục',
      author: 'Nguyễn Lê Thảo Nguyên',
    },
    {
      file: 'expose',
      name: 'Expose',
      author: 'Nguyễn Hoàng Long',
    },
    {
      file: 'ngoc-linh',
      name: 'Ngọc Linh',
      author: 'Nguyễn Phương Nhung',
    },
    {
      file: 'sinh-hoc-than-thu',
      name: 'Sinh Học Thần Thú',
      author: 'Nguyễn Đỗ Quỳnh Anh',
    },
    {
      file: 'timewise',
      name: 'Timewise',
      author: 'Nguyễn An Sơn',
    },
    {
      file: 'yeu-dau',
      name: 'Yêu Dấu',
      author: 'Nguyễn Đức Duy',
    },
  ];
</script>

<ul>
  <li>
    <a href="/projects/{projects[0].file}"
      ><img
        src="/thumbnails/{projects[0].file}.png"
        alt={projects[0].name}
      />{projects[0].name}<br />{projects[0].author}</a
    >
  </li>
  <li class="buffer"></li>
  <li>
    <a href="/projects/{projects[1].file}">
      <img
        src="/thumbnails/{projects[1].file}.png"
        alt={projects[1].name}
      />
      {projects[1].name}
      <br />
      {projects[1].author}
    </a>
  </li>
  <li>
    <a href="/projects/{projects[2].file}">
      <img
        src="/thumbnails/{projects[2].file}.png"
        alt={projects[2].name}
      />{projects[2].name}
      <br />
      {projects[2].author}
    </a>
  </li>

  <li class="buffer"></li>
  <li>
    <a href="/projects/{projects[3].file}">
      <img
        src="/thumbnails/{projects[3].file}.png"
        alt={projects[3].name}
      />
      {projects[3].name}
      <br />
      {projects[3].author}
    </a>
  </li>
  <li>
    <a href="/projects/{projects[4].file}">
      <img
        src="/thumbnails/{projects[4].file}.png"
        alt={projects[4].name}
      />
      {projects[4].name}
      <br />
      {projects[4].author}
    </a>
  </li>
  <li class="buffer"></li>

  <li>
    <a href="/projects/{projects[5].file}">
      <img
        src="/thumbnails/{projects[5].file}.png"
        alt={projects[5].name}
      />
      {projects[5].name}
      <br />
      {projects[5].author}
    </a>
  </li>
  <li>
    <a href="/projects/{projects[6].file}">
      <img
        src="/thumbnails/{projects[6].file}.png"
        alt={projects[6].name}
      />
      {projects[6].name}
      <br />
      {projects[6].author}
    </a>
  </li>
  <li class="buffer"></li>
  <li>
    <a href="/projects/{projects[7].file}">
      <img
        src="/thumbnails/{projects[7].file}.png"
        alt={projects[7].name}
      />
      {projects[7].name}
      <br />
      {projects[7].author}
    </a>
  </li>

  <li>
    <a href="/projects/{projects[8].file}">
      <img
        src="/thumbnails/{projects[8].file}.png"
        alt={projects[8].name}
      />
      {projects[8].name}
      <br />
      {projects[8].author}
    </a>
  </li>
  <li class="buffer"></li>
  <li>
    <a href="/projects/{projects[9].file}">
      <img
        src="/thumbnails/{projects[9].file}.png"
        alt={projects[9].name}
      />
      {projects[9].name}
      <br />
      {projects[9].author}
    </a>
  </li>
  <li>
    <a href="/projects/{projects[10].file}">
      <img
        src="/thumbnails/{projects[10].file}.png"
        alt={projects[10].name}
      />
      {projects[10].name}
      <br />
      {projects[10].author}
    </a>
  </li>
</ul>

<style>
  ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    gap: 15px;
    margin-top: 100px;
    margin-bottom: 100px;
    margin-right: 30px;
    padding-left: 30px;
    list-style: none;
  }

  img {
    width: 100%;
    margin-bottom: 12px;
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
</style>
