<template>
    <redoc-wrapper :spec-or-spec-url="'http://petstore.swagger.io/v2/swagger.json'" :options="redocOptions"></redoc-wrapper>
</template>

<script>
import RedocWrapper from '@/components/RedocWrapper'

export default {
  name: 'SpecUrlExample',
  components: {
    RedocWrapper
  },
  data() {
    return {
      // https://github.com/Redocly/redoc#redoc-options-object
      redocOptions: {
        hideDownloadButton: false
      }
    }
  }
}
</script>

<style scoped>

</style>