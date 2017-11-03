<template>
  <div class="line" ref="line" :style="{background:bg,width:linewidth,heigth:lineheight}"></div>
</template>

<script>
  export default {
    props: ['bg','linewidth','lineheight']
  }
</script>

<style lang="scss" scoped>
  .line {
    width: 60%;
    height: 1px;
    background-color: rgba(255,255,255,0.1);
  }
</style>