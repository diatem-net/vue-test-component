# Diatem | Vue Test Component

Just a Vue 3 proof-of-concept test component.

## Features

## Installation

```bash
npm i @diatem-net/vue-test-component
```

## How to Use

### Global Registration
main.js
```javascript
import TestComponent from '@diatem-net/vue-test-component'
import '@diatem-net/vue-test-component/dist/style.css'

createApp(App)
  .use(router)
  .use(TestComponent)
  .mount("#app");
```
#### OR

### Local Registration
HelloWorld.vue
```vue
<script setup>
import TestComponent from '@diatem-net/vue-test-component'
import '@diatem-net/vue-test-component/dist/style.css'

<template>
  <TestComponent msg="Hello world 😄" />
</template>

</script>
```
