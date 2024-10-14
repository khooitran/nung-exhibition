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
      file: 'cultural-archives',
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
  {#each projects as project}
    <a href="/projects/{project.file}"
      ><img
        src="/thumbnails/{project.file}.png"
        alt=""
      />{project.name} by {project.author}</a
    >
  {/each}
</ul>

<style>
  ul {
    display: grid;
    grid-template-columns: auto auto auto auto;
    margin-top: 100px;
  }
  img {
    width: 100%;
  }
</style>
