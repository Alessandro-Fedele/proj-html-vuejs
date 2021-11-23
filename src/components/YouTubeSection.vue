<template>
  <div class="container-fluid px-0 section-3 clearfix position-relative">
    <div class="position-absolute card-yt">
      <a href="#" class="play-button">
        <i class="fa fa-play" aria-hidden="true"></i>
      </a>
    </div>
    <div class="yt-section float-end">
      <h2>Tune up your workouts</h2>
      <h1>The best heatlh &amp; fitness advice online</h1>
      <div class="d-flex mb-4">
        <img src="@/assets/img/unnamed.jpg" alt="logo" class="me-2" />
        <div class="themeFusion">
          <div class="pb-1">ThemeFusion</div>
          <div>
            <button type="button" class="btn rounded-start px-1 py-0">
              <i class="fa fa-youtube-play pe-2" aria-hidden="true"></i>YouTube
            </button>
            <span class="ps-2">999+</span>
          </div>
        </div>
      </div>
      <p>
        Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper mauris,
        venenatis, leo integer sit pellenteque.
      </p>
      <button
        type="button"
        class="btn btn-primary rounded-pill btn-blu-style btn-pad"
      >
        <i class="fa fa-youtube-play pe-2" aria-hidden="true"></i> Visit my
        YouTube channel
      </button>
    </div>
  </div>
</template>
<script>
export default {
  name: "YouTubeSection",
};
</script>