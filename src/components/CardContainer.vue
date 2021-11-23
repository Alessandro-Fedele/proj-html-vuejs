<template>
  <div class="container-fluid section-2 position-relative">
    <div class="ab-card container position-absolute">
      <div class="row g-5">
        <Card
          v-for="(card, i) in cardList"
          :key="i"
          :imgUrl="card.imgUrl"
          :title="card.title"
          :text="card.text"
        ></Card>
      </div>
    </div>
    <div class="container s2-container text-center">
      <p>
        "How you respond to the challenge in the second half will determine what
        you become after the game, whether you are a winner or a lose."
      </p>
      <img src="@/assets/img/zigzag.png" alt="separator" />
      <div class="d-flex avatar-cont justify-content-center">
        <img src="@/assets/img/avatar-1-2x.jpg" alt="avatar" />
        <span class="pe-3">Brad Johnson</span>
        <span class="ls">Las Vegas</span>
      </div>
    </div>
  </div>
</template>
<script>
import Card from "@/components/Card";
export default {
  name: "CardContainer",
  components: { Card },
  data() {
    return {
      cardList: [
        {
          title: "Crossfit workout",
          text: "Push your limits",
          imgUrl: require("@/assets/img/service6-2x.jpg"),
        },
        {
          title: "New gym apparel",
          text: "Look good, feel good",
          imgUrl: require("@/assets/img/box1-2x.jpg"),
        },
        {
          title: "Team training",
          text: "Find a Partner",
          imgUrl: require("@/assets/img/box3-2x.jpg"),
        },
      ],
    };
  },
};
</script>