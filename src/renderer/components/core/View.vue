<template >
  <div :class="$style.view">
    <transition enter-active-class="animated-fast fadeIn"
    leave-active-class="animated-fast fadeOut"></transition>
    <router-view/>
  </div>

</template>


<style lang="less" module>
@import '../../assets/styles/layout.less';

.view {
  position: relative;
  z-index: 1;
  > * {
    position: absolute;
    width: 100%;
  }
  // background: #fff;
  // overflow: hidden;
}

</style>
