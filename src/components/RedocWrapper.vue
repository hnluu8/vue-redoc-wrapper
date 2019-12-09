<template>
  <div id="redoc-container"></div>
</template>

<script>
import * as redoc from 'redoc/bundles/redoc.standalone'

export default {
  name: "RedocWrapper",
  props: ['specOrSpecUrl', 'options'],
  data() {
    return {
      options_: {
        scrollYOffset: 50,
        hideDownloadButton: true
      }
    }
  },
  created() {
    if (this.options) {
      this.options_ = Object.assign(this.options_, this.options)
    }
  },
  mounted() {
    redoc.init(this.specOrSpecUrl, this.options_, document.getElementById('redoc-container'))
  }
}
</script>

<style scoped>

</style>