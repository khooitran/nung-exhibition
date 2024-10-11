<script>
  import AboutUs from '../lib/AboutUs.svelte';
  import HeroSection from '../lib/HeroSection.svelte';
  import Projects from '../lib/Projects.svelte';

  let images = [
    'dangquocanh.png',
    'dinhsonglinh.png',
    'doanminhquan.png',
    'dohanhmi.png',
    'hoanglong.png',
    'hungson.png',
    'nguyenanson.png',
    'nguyendoquynhanh.png',
    'nguyenducduy.png',
    'phuongnhung.png',
    'quynhhuong.png',
    'thaonguyen.png',
    'thuhai.png',
    'thuytrang.png',
    'trankhanhlinh.png',
    'tubaongan.png',
  ];

  let reversedImages = images.toReversed();
</script>

<HeroSection />

<section>
  <div class="image-rows">
    {#each images as image}
      <img
        src="/tiles/{image}"
        alt="one of the personal tiles of the 16 designers, reflecting their philosophy and style in design."
      />
    {/each}
  </div>
  <div class="content">
    <AboutUs />
    <Projects />
  </div>
  <div class="image-rows">
    {#each reversedImages as reversedImage}
      <img
        src="/tiles/{reversedImage}"
        alt="one of the personal tiles of the 16 designers, reflecting their philosophy and style in design."
      />
    {/each}
  </div>
</section>

<style>
  section {
    height: 92vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .content {
    display: flex;
    justify-content: space-between;
  }

  .image-rows {
    display: grid;
    grid-template-columns: auto auto auto auto auto auto auto auto auto auto auto auto auto auto auto auto;
    gap: 8px;
    margin: 30px;
  }

  img {
    width: 100%;
    height: auto;
  }

  @media only screen and (orientation: portrait) {
    section {
      height: fit-content;
    }
  }

  @media only screen and (max-width: 576px) {
    .image-rows {
      grid-template-columns: auto auto auto auto auto auto auto auto;
    }

    img:nth-child(even) {
      display: none;
    }

    .content {
      flex-direction: column;
    }
  }
</style>
