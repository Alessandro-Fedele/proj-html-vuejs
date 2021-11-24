<template>
  <div class="container-fluid footer-section">
    <div class="container mrgbot">
      <div class="row">
        <div class="col-4">
          <img src="@/assets/img/logo.png" alt="logo" />
          <p class="left-p">
            Ac aliquam neque sagittis diam faucibus vitae purus turpis
            phasellus. Pellentesque consectetur amet purus ultrices mauris.
          </p>
          <div class="d-flex social-cont">
            <i class="fa fa-facebook" aria-hidden="true"></i>
            <i class="fa fa-twitter" aria-hidden="true"></i>
            <i class="fa fa-youtube-play" aria-hidden="true"></i>
            <i class="fa fa-instagram" aria-hidden="true"></i>
            <i class="fa fa-linkedin" aria-hidden="true"></i>
          </div>
        </div>
        <div class="col-4">
          <h2>RECENT POSTS</h2>
          <ul class="text-center pe-4">
            <li v-for="(link, i) in footerlinkList" :key="i">
              <a href="#">
                <i class="fa fa-chevron-right" aria-hidden="true"></i>
                {{ link.text }}
              </a>
            </li>
          </ul>
        </div>
        <div class="col-4">
          <h2>CONTACT INFORMATIONS</h2>
          <h3>4746 Tipple Road Michigan 48449</h3>
          <p class="right-p">
            Mobile:1.800.000.0000<br />Email:info@your-company.com
          </p>
        </div>
      </div>
    </div>
    <div><hr /></div>
    <div class="container text-center foot-text">
      <i class="fa fa-copyright" aria-hidden="true"></i> Copyright 2012 - 2020 |
      Avada theme by <a href="#">ThemeFusion</a> ! All rights reserved | Powered
      by <a href="#">Boolean</a>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
  data() {
    return {
      footerlinkList: [
        {
          text: "The best protein shake",
        },
        {
          text: "Ultimate cardio workout",
        },
        {
          text: "New juices available now",
        },
        {
          text: "Tips to find training partners",
        },
        {
          text: "20 best healthy recipes",
        },
      ],
    };
  },
};
</script>