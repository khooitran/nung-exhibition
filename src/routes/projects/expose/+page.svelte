<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Nguyễn Hoàng Long',
    bio: "I am really into the grunge design style and have a strong interest in experimental design as well as animation - there's something incredible about bringing ideas to life through movement.",
    mail: 'longnolh@gmail.com',
    behance: 'https://www.behance.net/longremipsum',
    instagram: 'longremipsum',
  };

  let projectInfo = {
    file: 'expose',
    name: 'Expose',
    bio: 'Expose is an interactive visual experience that uncovers the truth behind misinformation. By blending chaotic design elements with immersive features like decoder magnifiers and lenticular cards, Expose challenges users to navigate the confusing world of false information. The project was designed for a conference on media literacy and aims to encourage critical thinking, engagement, and awareness in a world where truth is often hidden among lies.',
    images: [
      ['1.JPG', '2.JPG', '3.JPG'],
      ['4.JPG', '5.JPG', '6.JPG'],
      ['7.JPG', '8.JPG', '9.JPG'],
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
