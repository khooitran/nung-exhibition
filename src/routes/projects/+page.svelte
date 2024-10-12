<script>
  let projects = [
    {
      file: 'bach-khoa-khong-toan-thu',
      name: 'Bách Khoa Không Toàn Thư',
      author: 'Trần Khánh Linh',
    },
    {
      file: 'algorithmic-beauty',
      name: 'Algorithmic Beauty',
      author: 'Từ Bảo Ngân',
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
