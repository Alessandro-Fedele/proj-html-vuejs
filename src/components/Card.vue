<template>
  <div class="col-4">
    <div class="card">
      <img :src="imgUrl" :alt="title" />
      <div class="overlay"></div>
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