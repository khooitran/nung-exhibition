<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Nguyễn Thu Hải',
    bio: 'Hi, I am a graphic designer specializing in creating visually appealing and engaging brand identities, packaging designs and typography.',
    mail: 'ngthuha034@gmail.com',
    behance: 'https://www.behance.net/thuhanguyen15',
  };

  let projectInfo = {
    file: 'adopt-to-adore',
    name: 'Adopt to Adore',
    bio: 'Adopt & Adore is a social campaign with the aim of persuading people to adopt pets from adoption shelters with playful and energertic vibes. By humanizing pets in a funny way and linking their roles in life into a human job, I want to emphasize the benefit of having pets that make our life become more vibrant.',
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
