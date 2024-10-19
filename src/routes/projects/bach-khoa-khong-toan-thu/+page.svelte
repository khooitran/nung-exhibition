<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Trần Khánh Linh',
    bio: 'My strengths are editorial, illustration and 2D graphic design. I believe visual can be a powerful language to connect and engage the communities.',
    mail: 'khanhlinh2002bg@gmail.com',
    behance: 'https://www.behance.net/tranlinh40',
  };

  let projectInfo = {
    file: 'bach-khoa-khong-toan-thu',
    name: 'Bách Khoa Không Toàn Thư',
    bio: "The book is part of a series depicting Vietnamese childhoods through visual language. By focusing on children's experiences, the project aims to connect with young Vietnamese who have to go far from their homeland and help foreigners understand Vietnamese culture and. From that, building a community about Vietnam childhood topic.",
    images: [
      ['1.png', '2.png', '3.png'],
      ['4.png', '5.png', '6.png'],
      ['7.png', '8.png', '9.png'],
    ],
  };
</script>

<section>
  <div class="buffer"></div>
  <div class="project-section">
    <Content {...projectInfo} />
    <Collage {...projectInfo} />
  </div>
  <AuthorInfo {...authorInfo} />
</section>

<style>
  section {
    margin: 100px 30px;
    display: grid;
    grid-template-columns: 1fr 2.5fr;
  }

  @media only screen and (max-width: 992px) {
    .buffer {
      display: none;
    }

    section {
      grid-template-columns: 1fr;
    }
  }
</style>
