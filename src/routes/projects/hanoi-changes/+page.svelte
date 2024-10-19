<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Nguyễn Đặng Hùng Sơn',
    bio: 'I am a graphic designer based in Hanoi, Vietnam. My majors are Graphic Design and UI/UX Design.',
    mail: 'hson7593@gmail.com',
    behance: 'https://www.behance.net/hungson2',
    instagram: 'byhson._',
  };

  let projectInfo = {
    file: 'hanoi-changes',
    name: 'Hanoi Changes',
    bio: "Hanoi's history and culture are its distinctive traits, but rapid modernization is causing these old values to fade, especially among the youth. This project highlights the city's changes and celebrates its local history through three main historical periods, thereby bridging the cultural gap created by globalization.",
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

  @media only screen and (max-width: 768px) {
    .buffer {
      display: none;
    }

    section {
      grid-template-columns: 1fr;
    }
  }
</style>
