<template>
  <div class="container playlist">
    <div class="d-flex justify-content-between">
      <h2>Featured playlists</h2>
      <a href="#" class="yt-link">
        <span
          >View all videos
          <i class="fa fa-angle-right ps-2" aria-hidden="true"></i
        ></span>
      </a>
    </div>
    <div class="row g5">
      <div class="col-4" v-for="(card, i) in videoPrevList" :key="i">
        <div class="card">
          <img :src="card.imgUrl" class="card-img-top mb-2" alt="logo" />
          <a href="#" class="play-button">
            <i class="fa fa-play" aria-hidden="true"></i>
          </a>
          <div class="card-body">
            <h4 class="card-title">{{ card.title }}</h4>
            <p class="card-text">
              {{ card.text }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "PlaylistCard",
  data() {
    return {
      videoPrevList: [
        {
          imgUrl: require("@/assets/img/video2-2x.jpg"),
          title: "Thighs & glute workout",
          text: "Increase your mobility",
        },
        {
          imgUrl: require("@/assets/img/video7-2x.jpg"),
          title: "Lift, firm & perk up",
          text: "Feel young again",
        },
        {
          imgUrl: require("@/assets/img/video9-2x.jpg"),
          title: "Slim & trim your waist",
          text: "Shed those extra pounds",
        },
      ],
    };
  },
};
</script>