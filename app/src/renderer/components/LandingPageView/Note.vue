<template>
    <div ref="main" id="main">
        <div v-on:click="move" ref="sidebar" class="sidebar"></div>
    </div>
</template>

<script>
  export default {
    data () {
      return {}
    },
    methods: {
      move: function (e) {
        e.preventDefault()
        console.log('HIHIHI')
//        dragging = true;
        let main = $('#main')
        let ghostbar = $('<div>',
          {
            id: 'ghostbar',
            css: {
              height: main.outerHeight(),
              top: main.offset().top,
              left: main.offset().left
            }
          }).appendTo('body')

        $(document).mousemove(function (e) {
          ghostbar.css('left', e.pageX + 2)
        })
      }
    }
  }
</script>

<style lang="scss" scoped>
    div {
        height: 100vh;
        width: 10vw;
        background: #3c3f41;
        float: left;
        &.sidebar {
            background-color: black;
            height: 100%;
            float: right;
            width: 3px;
            cursor: col-resize;
        }
    }
</style>
