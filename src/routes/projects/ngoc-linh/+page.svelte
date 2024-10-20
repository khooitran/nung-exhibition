<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';
  import Video from '../../../lib/Video.svelte';

  let authorInfo = {
    name: 'Nguyễn Phương Nhung',
    bio: "I'm Nhung, an illustrator and designer based in Hanoi, Vietnam. I'm passionate and skilled in illustration, 3D modelling, and animation. My art style is often described as dreamy, whimsical, and distinctly Vietnamese.",
    mail: 'nhoongmeep@outlook.com',
    behance: 'https://www.behance.net/nhoongmeep',
    instagram: 'nhoongmeepbkl',
  };

  let projectInfo = {
    file: 'ngoc-linh',
    name: 'Ngọc Linh',
    bio: 'Ngọc Linh: Roots to the Past is a game designed to inspire young generations in Vietnam to rediscover their heritage and traditional values. Join Ngọc Linh, a young woman struggling with her identity, on a journey to the past. Through this adventure, players will explore creativity, gather memories, and confront the challenges of preserving traditional crafts. Using a journal and traditional art mediums, you will delve into the past, present, and future of cultural conservation.',
    images: [
      ['1.png', '2.jpg', '3.jpg'],
      ['4.jpg', '5.jpg', '6.jpg'],
      ['7.jpg', '8.png', '9.png'],
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
      title="flipbook"
      allowfullscreen="allowfullscreen"
      scrolling="no"
      src="https://heyzine.com/flip-book/b15416dab8.html"
      style="border: 1px solid lightgray; width: 100%; height: 600px;"
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
