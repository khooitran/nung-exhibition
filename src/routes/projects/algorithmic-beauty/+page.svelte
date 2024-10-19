<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Từ Bảo Ngân',
    bio: 'I am a graphic designer with a strong passion for editorial and layout design, a love for developing brand identities, and a solid foundation in UI/UX design.',
    mail: 'nagn.naci@gmail.com',
    website: 'https://www.naci.cargo.site',
  };

  let projectInfo = {
    file: 'algorithmic-beauty',
    name: 'Algorithmic Beauty',
    bio: 'We all subconsciously adjust our appearance based on personal beauty standards. Algorithmic Beauty explores how digital algorithms promote unattainable beauty from historical roots to modern ideals, highlighting the impact of social media and data trends on unattainable benchmarks, questioning readers about their view of beauty.',
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
