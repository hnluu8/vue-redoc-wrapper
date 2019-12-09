# vue-redoc-wrapper
A Vue.js wrapper component for [ReDoc](https://github.com/Redocly/redoc).

[![npm package](https://img.shields.io/npm/v/@hnluu8/vue-redoc-wrapper.svg?style=flat-square)](https://www.npmjs.com/package/@hnluu8/vue-redoc-wrapper)

## Installation
```bash
npm install @hnluu8/vue-redoc-wrapper --save
```

## Usage
Pass the [OpenAPI definitions](https://swagger.io/specification/#schema) for your API to the spec-or-spec-url attribute of the component. 
The attribute value can be given as an object or as a URL to the JSON or YAML file of your API documentation. 

```html
<template>
  <div id="app">
    <redoc-wrapper :spec-or-spec-url="'http://petstore.swagger.io/v2/swagger.json'"></redoc-wrapper>
  </div>
</template>

<script>
import RedocWrapper from '@hnluu8/vue-redoc-wrapper'

export default {
  name: 'app',
  components: {
    RedocWrapper
  }
}
</script>
```

### Component Props
The component exposes two props: _specOrSpecUrl_ (required) and _options_ (optional). Please visit the documentation for 
[ReDoc's standalone version](https://github.com/Redocly/redoc#advanced-usage-of-standalone-version) for more information on their usage.


## Demo
```bash
vue serve demo/components/SpecUrlExample.vue
```