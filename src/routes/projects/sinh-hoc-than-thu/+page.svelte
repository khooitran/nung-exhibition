<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Ng. Ngọc Quỳnh Hương',
    bio: "I'm Hương, a 2D artist specializing in digital art with 2 years of working experience producing outcomes in a wide range of illustration styles, from stylized to photo-realism.",
    mail: 'quynhhuong.nguyen2001@gmail.com',
    behance: 'https://www.behance.net/huongnguyen358',
  };

  let projectInfo = {
    file: 'sinh-hoc-than-thu',
    name: 'Sinh Học Thần Thú',
    bio: 'Sinh Học Thần Thú - Rồng is part of a larger book series titled Sinh Học Thần Thú, designed to introduce basic animal biology to young students aged 5 to 10 by examining the body parts of holy beasts and mythological creatures. In this volume, the Vietnamese Dragon serves as a visual and educational tool to explore real-world animal anatomy and biology in a fun and engaging way. By combining elements of mythology and science, the project aims to make learning biology more accessible and less intimidating for children, sparking curiosity and fostering a love for the natural world.',
    images: [
      ['1.png', '2.png', '3.png'],
      ['4.png', '5.png', '6.png'],
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
