<template>
    <redoc-wrapper :spec-or-spec-url="spec"></redoc-wrapper>
</template>

<script>
import RedocWrapper from '@/components/RedocWrapper'

export default {
  name: 'SpecExample',
  components: {
    RedocWrapper
  },
  data() {
    return {
      spec: {
        openapi: "3.0.2",
        servers: [
          {
            url: "https://try-api.loominus.ai"
          }
        ],
        info: {
          description: "Don't have an API Key? [[Register]](https://try.loominus.ai/register)",
          title: "Loominus API",
          version: "1.0.0"
        },
        paths: {
        }
      }
    }
  }
}
</script>

<style scoped>

</style>