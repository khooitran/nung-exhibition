<script>
  export let file;
  export let video;
</script>

<!-- svelte-ignore a11y-media-has-caption -->
<video
  src="/individuals/{file}/{video}"
  controls
  width="100%"
  height="auto"
>
  Your browser does not support video feature.
</video>
