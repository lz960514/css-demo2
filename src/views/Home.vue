<template>
  <div class="home">
    <stripLoading></stripLoading>
    <h1>条形加载条</h1>
    <heartLoading></heartLoading>
    <h1>心形加载条</h1>
    <tabNavbar></tabNavbar>
    <h1>标签导航栏</h1>
    <trackBtn></trackBtn>
    <h1>妙用CSS变量，让你的CSS变得更心动</h1>
    <parallaxBtn></parallaxBtn>
    <h1>妙用CSS变量，让你的CSS变得更心动</h1>
    <likeBtn></likeBtn>
  </div>
</template>
<script>
// @ is an alias to /src

import stripLoading from "../components/strip-loading/index";

import heartLoading from "../components/heart-loading/index";

import tabNavbar from "../components/tab-navbar/index";

import trackBtn from "../components/track-btn/index";

import parallaxBtn from "../components/parallax-btn/index";

import likeBtn from "../components/like-btn/index";

export default {
  name: "Home",
  components: {
    stripLoading,
    heartLoading,
    tabNavbar,
    trackBtn,
    parallaxBtn,
    likeBtn,
  },
};
</script>

<style lang="scss" scoped>
h1 {
  margin: 10px 0;
}
</style>
