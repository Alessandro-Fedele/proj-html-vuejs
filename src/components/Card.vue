<template>
  <div class="col-4">
    <div class="card">
      <img :src="imgUrl" :alt="title" />
      <div class="overlay">
        <div class="position-relative">
          <img
            class="separator"
            src="@/assets/img/zigzag-white.png"
            alt="separator"
          />
          <h2>{{ title }}</h2>
          <h3>{{ text }}</h3>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Card",
  props: {
    title: String,
    text: String,
    imgUrl: String,
  },
};
</script>