<template>
    <div>
        <div class="sidebar"></div>
    </div>
</template>

<script>
  export default {
    data () {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
    div {
        width: 20vw;
        background: #3c3f41;
        float: left;
        padding: 0;
        &.sidebar {
            background-color: black;
            height: 100%;
            float: right;
            width: 3px;
            cursor: col-resize;
        }
    }
</style>
