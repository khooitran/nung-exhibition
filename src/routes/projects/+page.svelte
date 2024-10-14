<script>
  import ProjectItem from '../../lib/ProjectItem.svelte';

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
  <li><ProjectItem {...projects[0]} /></li>
  <li class="buffer"></li>
  <li><ProjectItem {...projects[1]} /></li>
  <li><ProjectItem {...projects[2]} /></li>
  <li class="buffer"></li>
  <li><ProjectItem {...projects[3]} /></li>
  <li><ProjectItem {...projects[4]} /></li>
  <li class="buffer"></li>
  <li><ProjectItem {...projects[5]} /></li>
  <li><ProjectItem {...projects[6]} /></li>
  <li class="buffer"></li>
  <li><ProjectItem {...projects[7]} /></li>
  <li><ProjectItem {...projects[8]} /></li>
  <li class="buffer"></li>
  <li><ProjectItem {...projects[9]} /></li>
  <li><ProjectItem {...projects[10]} /></li>
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
</style>
