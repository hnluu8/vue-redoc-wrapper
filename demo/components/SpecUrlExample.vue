<template>
    <redoc-wrapper :spec-or-spec-url="'http://petstore.swagger.io/v2/swagger.json'"></redoc-wrapper>
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