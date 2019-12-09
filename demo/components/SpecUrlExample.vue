<template>
    <redoc-wrapper :spec-or-spec-url="'/loominus-swagger.json'"></redoc-wrapper>
</template>

<script>
import RedocWrapper from '@/components/RedocWrapper'

export default {
  name: 'SpecUrlExample',
  components: {
    RedocWrapper
  }
}
</script>

<style scoped>

</style>