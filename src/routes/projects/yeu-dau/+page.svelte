<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';
  import Video from '../../../lib/Video.svelte';

  let authorInfo = {
    name: 'Nguyễn Đức Duy',
    bio: 'I am a graphic designer based in Hanoi, Vietnam, specializing in Graphics, Motion Graphics and Typography.',
    mail: 'duaymusic@gmail.com',
    behance: 'https://www.behance.net/duynguyendxy',
    website: 'https://duynguyendxy.cargo.site',
  };

  let projectInfo = {
    file: 'yeu-dau',
    name: 'Yêu Dấu',
    bio: 'Yêu Dấu aims to help people in all ages learn the Vietnamese tone system using interactive and visually appealing graphic, and easy-to-follow lessons through a scan from the phone. This work placed in the context of the lack of standardized Vietnamese language learning guide for foreigners, which can work in many circumstances.',
    images: [
      ['1.gif', '2.png', '3.png'],
      ['4.png', '5.gif', '6.png'],
      ['7.gif', '8.png', '9.jpg'],
    ],
    video: '03.webm',
  };
</script>

<section>
  <div class="buffer"></div>
  <div class="project-section">
    <Content {...projectInfo} />
    <Video {...projectInfo} />
    <video
      src="/individuals/{projectInfo.file}/02.webm"
      autoplay
      muted
      width="100%"
      height="auto"
    >
      Your browser does not support video feature.
    </video>
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
