<template>
    <div id="app">
        <router-view></router-view>
    </div>
</template>

<script>
  import store from 'renderer/vuex/store'
  export default {
    store
  }
</script>

<style lang="sass">
    @import url(https://fonts.googleapis.com/css?family=Lato:300);

    *
        margin: 0
        padding: 0

    div
        height: 100vh
        overflow: hidden
        &#app
            background: #8b8bff

    /*align-items: center;*/
    /*background: radial-gradient(*/
    /*ellipse at center,*/
    /*rgba(255, 255, 255, 1) 0%,*/
    /*rgba(229, 229, 229, .85) 100%*/
    /*) center;*/
    /*display: flex;*/
    /*font-family: Lato, Helvetica, sans-serif;*/
    /*justify-content: center;*/
    /*text-align: center;*/

</style>
