<template>
  <ul class="strip-loding flex-ct-x">
    <li v-for="(item, index) in 6" :key="index" :style="`--line-index:${ index }`"></li>
  </ul>
</template>

<script>
export default {
  name: "strip-loading",
};
</script>

<style lang="scss" scoped>
.strip-loding {
  width: 200px;
  height: 200px;
  li {
    --time: calc((var(--line-index) - 1) * 200ms);
    border-radius: 3px;
    width: 6px;
    height: 30px;
    background: #f66;
    animation: beat 1.5s ease-in-out var(--time) infinite;
    & + li {
      margin-left: 5px;
    }
  }
}

@keyframes beat {
  0%,
  100% {
    transform: scaleY(1);
  }
  50% {
    transform: scaleY(0.5);
  }
}
</style>