<template>
  <div class="container-fluid black-cont">
    <div class="container">
      <div class="row g-5">
        <div class="col-4" v-for="(card, i) in planList" :key="i">
          <div class="card">
            <img :src="card.imgUrl" class="card-img-top mb-3" alt="logo" />
            <div class="card-body">
              <h2 class="card-title mb-3">{{ card.title }}</h2>
              <h4 class="mb-4">{{ card.subtitle }}</h4>
              <p class="card-text">
                {{ card.text }}
              </p>
              <a href="#" class="my-link">
                <span
                  >{{ card.link }}
                  <i class="fa fa-angle-right ps-2" aria-hidden="true"></i
                ></span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "PlanCard",
  data() {
    return {
      planList: [
        {
          imgUrl: require("@/assets/img/sport-watch.png"),
          title: "Team Training",
          subtitle: "Find a partner",
          text: "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehicula. Tristique.",
          link: "Find a partner",
        },
        {
          imgUrl: require("@/assets/img/gym.png"),
          title: "Crossfit workout",
          subtitle: "Push your limits",
          text: "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehicula. Tristique.",
          link: "Learn about Crossfit",
        },
        {
          imgUrl: require("@/assets/img/fitness.png"),
          title: "Weight loss plan",
          subtitle: "Shed those pounds",
          text: "At laoreet senectus volutpat diam vel sed sed amet pellentesque. Lobortis ut aliquam risus purus. A tellus ut etiam",
          link: "Schedule a workout",
        },
      ],
    };
  },
};
</script>