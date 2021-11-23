<template>
  <div class="container articles">
    <div class="d-flex justify-content-between">
      <h2>Latest articles</h2>
      <a href="#" class="my-link">
        <span
          >Read all articles
          <i class="fa fa-angle-right ps-2" aria-hidden="true"></i
        ></span>
      </a>
    </div>
    <div class="row g-5">
      <div class="col-4" v-for="(card, i) in articlePrevList" :key="i">
        <div class="card">
          <img
            :src="card.imgUrl"
            class="card-img-top mb-2 position-relative"
            alt="logo"
          />
          <div class="overlay"></div>
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
  name: "ArticleCard",
  data() {
    return {
      articlePrevList: [
        {
          imgUrl: require("@/assets/img/blog4-2x.jpg"),
          title: "The best protein shake",
          text: "By admin | November 26th, 2019 | Gym",
        },
        {
          imgUrl: require("@/assets/img/blog1-2x.jpg"),
          title: "Ultimate cardio workout",
          text: "By admin | November 26th, 2019 | Gym",
        },
        {
          imgUrl: require("@/assets/img/blog3-2x.jpg"),
          title: "New juices available now",
          text: "By admin | November 26th, 2019 | Gym",
        },
      ],
    };
  },
};
</script>