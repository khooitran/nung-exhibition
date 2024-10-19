<script>
  import AuthorInfo from '../../../lib/AuthorInfo.svelte';
  import Content from '../../../lib/Content.svelte';
  import Collage from '../../../lib/Collage.svelte';

  let authorInfo = {
    name: 'Nguyễn An Sơn',
    bio: "Hello there! I am a graphic/visual designer and photographer based in Hanoi. I strive to create design that understand and focus on user's needs, commiting to deliver aesthetically pleasing and functional designs.",
    mail: 'sn.nguyen.hn@gmail.com',
    behance: 'https://www.behance.net/snnguyenhn',
    instagram: 'sn.nguyen.hn',
  };

  let projectInfo = {
    file: 'timewise',
    name: 'Timewise',
    bio: 'Timewise is a time management and to-do list app project that aims to strive for both work efficiency and work-life-break time ratio balanced through time boxing and session breaks, promoting healthy working habits by letting the user assign a certain number of tasks for the day and helping users breaking down tasks to subtasks.',
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
