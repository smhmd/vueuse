<!--DEMO_STARTS--><!--DEMO_ENDS-->

<!--HEAD_STARTS--><!--HEAD_ENDS-->

# useUrlSearchParams

> Reactive [URLSearchParams](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams)

## Usage

```html {19}
<template>
  <ul>
    <li v-for='key in Object.keys(params)'>{{ key }}={{ params[key] }}</li>
  </ul>
</template>

<script>
import { useUrlSearchParams } from '@vueuse/core'

export default {
  setup() {
    const params = useUrlSearchParams('history')
    params.foo = 'bar'
    return { params }
  } 
}
</script>
```


<!--FOOTER_STARTS-->


## Source

[Source](https://github.com/antfu/vueuse/blob/master/packages/core/useUrlSearchParams/index.ts) • [Docs](https://github.com/antfu/vueuse/blob/master/packages/core/useUrlSearchParams/index.md)


<!--FOOTER_ENDS-->