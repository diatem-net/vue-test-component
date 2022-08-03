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
import ColorPicker from '@mcistudio/vue-colorpicker'
import '@mcistudio/vue-colorpicker/style.css'
createApp(App)
  .use(router)
  .use(ColorPicker)
  .mount("#app");
```
#### OR

### Local Registration
HelloWorld.vue
```vue
<script setup>
import ColorPicker from '@mcistudio/vue-colorpicker'
import '@mcistudio/vue-colorpicker/dist/style.css'

<template>
  <ColorPicker></ColorPicker>
</template>

</script>
```

### demo
HelloWorld.vue
```vue
<template>
  <ColorPicker mode="mode" :degree="degree" :gradients="grad" @colorChanged="triggerChanged" />
</template>

<script setup>
import ColorPicker from '@mcisutdio/vue-colorpicker'
import '@mcisutdio/vue-colorpicker/dist/style.css'
import { ref } from 'vue'
const mode = ref('linear')
const degree = ref(90)
const grad = ref([
  { id: 0, percent: 10, color: { r: 255, g: 10, b: 20, a: 1 } },
  { id: 1, percent: 100, color: { r: 59, g: 50, b: 240, a: 1 } },
])
function triggerChanged(color) {
  console.log('current color:', color)
}
</script>
```



