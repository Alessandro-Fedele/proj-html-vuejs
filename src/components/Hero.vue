<template>
  <div class="container-fluid hero d-flex position-relative">
    <div class="container">
      <div class="row">
        <div class="col-8">
          <h2 class="pb-2">Certified fitness professional</h2>
          <h1>Take control of your health</h1>
          <img
            class="separator"
            src="@/assets/img/zigzag.png"
            alt="separator"
          />
          <p class="pb-4">
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectus
            dolor sit amet.
          </p>
          <div class="d-flex">
            <button
              type="button"
              class="btn btn-primary rounded-pill btn-blu-style btn-pad me-3"
            >
              <i class="fa fa-youtube-play pe-2" aria-hidden="true"></i> Visit
              my YouTube channel
            </button>
            <button type="button" class="btn btn-dark rounded-pill btn-pad">
              Buy Avada today
              <i class="fa fa-arrow-right ps-2" aria-hidden="true"></i>
            </button>
          </div>
        </div>
        <div class="col-4 d-flex justify-content-center align-items-center">
          <a href="#" class="play-button playmarg">
            <i class="fa fa-play" aria-hidden="true"></i>
          </a>
        </div>
      </div>
    </div>
    <!-- <div class="position-absolute demos">
      <a href="#">
        <i class="fa fa-folder" aria-hidden="true"></i>
      </a>
      <a href="#">
        <i class="fa fa-folder" aria-hidden="true"></i>
      </a>
    </div> -->
  </div>
</template>
<script>
export default {
  name: "Hero",
};
</script>