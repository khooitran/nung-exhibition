<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Đinh Song Linh',
    bio: 'A mixed-media Artist/Designer, focusing on improving the Mixed-media part right now. Currently obsessed with stop-motion animation, Massive Attack, and Brutalist Architecture',
    mail: 'lilbom1227@gmail.com',
    behance: 'https://www.behance.net/linhdinhsong',
    instagram: 'yohjiyamamotoismydad_',
  };

  let projectInfo = {
    file: 'cultural-archive',
    name: 'Cultural Archive: Ethnicities',
    bio: `Culture Archive: Ethnicities is an archive website that documents and digitize cultural artefacts of ethnic groups in Vietnam, with the goal to motivate people to learn about ethnic minorities and persuade them to engage in preserving and growing ethinc culture. The project chose the Hmong group as its self-produced illustrations.`,
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
