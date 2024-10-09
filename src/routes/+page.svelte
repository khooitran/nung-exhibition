<script>
  import AboutUs from '../lib/AboutUs.svelte';
  import HeroSection from '../lib/HeroSection.svelte';
  import Projects from '../lib/Projects.svelte';
</script>

<HeroSection />

<div class="navigation">
  <div class="image-rows">
    <img
      src="/tiles/dangquocanh.png"
      alt=""
    />
    <img
      src="/tiles/dinhsonglinh.png"
      alt=""
    />
    <img
      src="/tiles/doanminhquan.png"
      alt=""
    />
    <img
      src="/tiles/dohanhmi.png"
      alt=""
    />
    <img
      src="/tiles/hoanglong.png"
      alt=""
    />
    <img
      src="/tiles/hungson.png"
      alt=""
    />
    <img
      src="/tiles/nguyenanson.png"
      alt=""
    />
    <img
      src="/tiles/nguyendoquynhanh.png"
      alt=""
    />
  </div>
  <div class="content">
    <AboutUs />
    <Projects />
  </div>
  <div class="image-rows">
    <img
      src="/tiles/nguyenducduy.png"
      alt=""
    />
    <img
      src="/tiles/phuongnhung.png"
      alt=""
    />
    <img
      src="/tiles/quynhhuong.png"
      alt=""
    />
    <img
      src="/tiles/thaonguyen.png"
      alt=""
    />
    <img
      src="/tiles/thuhai.png"
      alt=""
    />
    <img
      src="/tiles/thuytrang.png"
      alt=""
    />
    <img
      src="/tiles/trankhanhlinh.png"
      alt=""
    />
    <img
      src="/tiles/tubaongan.png"
      alt=""
    />
  </div>
</div>

<style>
  .navigation {
    height: 92vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .content {
    display: flex;
    justify-content: space-between;
    padding-right: 30px;
  }

  .image-rows {
    display: grid;
    grid-template-columns: auto auto auto auto auto auto auto auto;
    gap: 8px;
    margin: 30px;
  }

  img {
    width: 100%;
    height: auto;
  }
</style>
