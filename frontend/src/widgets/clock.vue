<template lang="jade">
  div
    h1 {{date}}
    h2 {{time}}
</template>

<script>
  import Widget from './widget.js'

  export default {
    extends: Widget,

    data () {
      return {
        date: 0,
        time: 0
      }
    },
    mounted () {
      function formatTime (i) {
        if (i < 10) {
          return '0' + i
        } else {
          return i
        }
      }

      setInterval(() => {
        const today = new Date()
        const h = today.getHours()
        const m = formatTime(today.getMinutes())
        const s = formatTime(today.getSeconds())
        this.date = today.toLocaleDateString()
        this.time = `${h}:${m}:${s}`
      }, 500)
    }
  }
</script>

<style lang="stylus" scoped>
</style>
