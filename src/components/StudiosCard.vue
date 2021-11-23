<template>
  <div class="container-fluid sponsor-cont">
    <div class="container">
      <div class="row g-4">
        <div class="col-3" v-for="(card, i) in sponsorList" :key="i">
          <div class="card">
            <img :src="card.imgUrl" class="card-img-top mb-3" alt="logo" />
            <img
              class="separator"
              src="@/assets/img/zigzag-blu.png"
              alt="separator"
            />
            <div class="card-body">
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
  name: "StudiosCard",
  data() {
    return {
      sponsorList: [
        {
          imgUrl: require("@/assets/img/sponsor-1-2x.png"),
          text: "Tristique aliquam in nullam habitasse nunc, amet vel consectetur. Nulla in suspendisse dolr, aliquet.",
          link: "Visit Yoga Studio",
        },
        {
          imgUrl: require("@/assets/img/sponsor-2-2x.png"),
          text: "Feugiat etiam dui mauris pharetra mauris sed pharetra. Convallis sapien ornare cras faucibus nulla porta dui a.",
          link: "Join Fitness Center",
        },
        {
          imgUrl: require("@/assets/img/sponsor-3-2x.png"),
          text: "Nisl at quam adipiscing montes, nec, adipiscing commodo aliquam tincidunt. Ligula in habitant et sagittis imperdiet.",
          link: "Learn about FC",
        },
        {
          imgUrl: require("@/assets/img/sponsor-4-2x.png"),
          text: "Proin in viverra maecenas et mattis ut nibh enim. Gravida ultricies mi porta lacus. Et posuere velit sed nec eleifend.",
          link: "Visit Power Gym",
        },
      ],
    };
  },
};
</script>