<template>
    <div>
        <notebook></notebook>
        <div class="sidebar"></div>
        <note></note>
        <div class="sidebar"></div>
        <div class="ghostbar"></div>
        <editor></editor>
    </div>
</template>

<script>
  import Notebook from './LandingPageView/Notebook.vue'
  import Note from './LandingPageView/Note.vue'
  import Editor from './LandingPageView/Editor.vue'
  export default {
    components: {
      Notebook,
      Note,
      Editor
    },
    name: 'landing-page'
  }
</script>

<style scoped lang="sass">
    .sidebar
        background-color: black
        height: 100vh
        float: right
        width: 3px
        cursor: col-resize

    .ghostbar
        width: 3px
        background-color: #000
        opacity: 0.5
        position: absolute
        cursor: col-resize
        z-index: 999
</style>
