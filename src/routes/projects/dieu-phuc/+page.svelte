<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';
  import Video from '../../../lib/Video.svelte';

  let authorInfo = {
    name: 'Nguyễn Lê Thảo Nguyên',
    bio: 'I am a graphic designer based in Hanoi. I specialize in 2D graphics with a strong focus on: brand identity, packaging, UI design, 2D motion graphics, and graphic illustrations.',
    mail: 'nltnguyen0403@gmail.com',
    behance: 'https://www.behance.net/nltnguyen03',
    website: 'https://readymag.website/u3192193723/4951083',
  };

  let projectInfo = {
    file: 'dieu-phuc',
    name: 'Diệu Phục',
    bio: 'Vietnamese traditional clothing (or Cổ phục Việt/Việt phục) is a unique expression of Vietnamese culture and a cherished heritage of Vietnam. Yet, for much of modern history, these traditional garments, steeped in cultural and aesthetic value, have remained largely unknown to the wider public.  So, this project seeks to bridge that gap by designing an archive website - Diệu Phục - dedicated to supporting the preservation and dissemination of knowledge about Việt phục. The goal is to create an engaging, user-friendly digital platform that serves as a reliable resource for scholars, designers, and anyone interested in Việt phục.',
    images: [
      ['1.png', '2.png', '3.png'],
      ['4.png', '5.png', '6.png'],
      ['7.png', '8.png', '9.png'],
    ],
    video: 'video.webm',
  };
</script>

<section>
  <div class="buffer"></div>
  <div class="project-section">
    <Content {...projectInfo} />
    <Video {...projectInfo} />
    <iframe
      title="prototype"
      style="border: 1px solid rgba(0, 0, 0, 0.1);"
      width="100%"
      height="600px"
      src="https://embed.figma.com/proto/DIrmoVNFIynh4qyZxb2r37/Di%E1%BB%87u-Ph%E1%BB%A5c?page-id=0%3A1&node-id=27-131&node-type=canvas&viewport=241%2C295%2C0.02&scaling=scale-down-width&content-scaling=fixed&starting-point-node-id=408%3A3470&embed-host=share"
      allowfullscreen
    ></iframe>
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
