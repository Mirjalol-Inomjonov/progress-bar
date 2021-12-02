<template>
  <section class="progress-bar">
    <div class="progress-bar__inner">
      <span>100%</span>
    </div>
  </section>
</template>

<script>
export default {
  name: "Progressbar",
};
</script>

<style lang="scss" scoped>
.progress-bar {
  width: 100%;
  height: 20px;
  background: #fff;
  position: relative;
  &__inner {
    height: 100%;
    background: linear-gradient(to right, #ed008d, #2484e4);
    border-radius: 0 10px 10px 0;
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: #313131;
      font-size: 14px;
    }
  }
}
</style>
