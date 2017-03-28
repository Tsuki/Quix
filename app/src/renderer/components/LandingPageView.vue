<template>
    <div>
        <notebook>
            <div class="sidebar"></div>
        </notebook>
        <note>
            <div class="sidebar"></div>
        </note>
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

<style scoped lang="scss">
</style>
