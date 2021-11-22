<template>
  <nav class="navbar navbar-expand">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="@/assets/img/logo.png" alt="logo" />
      </a>
      <div class="d-flex">
        <ul class="navbar-nav">
          <li class="nav-item" v-for="(item, i) in navitemList" :key="i">
            <a
              class="nav-link"
              :class="item.active ? `active` : ``"
              :href="item.link"
              >{{ item.text }}</a
            >
          </li>
        </ul>
        <div class="new">new</div>
        <button
          type="button"
          class="btn btn-primary rounded-pill btn-blu-style"
        >
          Schedule a workout
        </button>
        <div class="icon-nav">
          <a href="#">
            <i class="fa fa-search" aria-hidden="true"></i>
          </a>
          <a href="#">
            <i class="fa fa-shopping-cart" aria-hidden="true"></i>
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "Navbar",
  data() {
    return {
      navitemList: [
        {
          link: "#",
          text: "Home",
          active: true,
        },
        {
          link: "#",
          text: "Services",
          active: false,
        },
        {
          link: "#",
          text: "About",
          active: false,
        },
        {
          link: "#",
          text: "Videos",
          active: false,
        },
        {
          link: "#",
          text: "Blog",
          active: false,
        },
        {
          link: "#",
          text: "Store",
          active: false,
        },
      ],
    };
  },
};
</script>