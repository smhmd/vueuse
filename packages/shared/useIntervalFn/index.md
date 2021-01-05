---
category: Animation
---

<!--DEMO_STARTS-->
<script setup>
import Demo from './demo.vue'
</script>
<DemoContainer><Demo/></DemoContainer>
<!--DEMO_ENDS-->

<!--HEAD_STARTS--><!--HEAD_ENDS-->


# useIntervalFn

> Wrapper for `setInterval` with controls

## Usage

```js
import { useIntervalFn } from '@vueuse/core'

const { start, stop } = useIntervalFn(() => {
  /* your function */
}, 1000)
```


<!--FOOTER_STARTS-->
## Type Declarations

```typescript
export interface IntervalFnReturn extends Pausable {
  /**
   * @deprecated use pause() instead
   */
  stop: Fn
  /**
   * @deprecated use resume() instead
   */
  start: Fn
}
/**
 * Wrapper for `setInterval` with controls
 *
 * @param cb
 * @param interval
 * @param immediate
 */
export declare function useIntervalFn(
  cb: Fn,
  interval?: number,
  immediate?: boolean
): IntervalFnReturn
```

## Source

[Source](https://github.com/antfu/vueuse/blob/master/packages/shared/useIntervalFn/index.ts) • [Demo](https://github.com/antfu/vueuse/blob/master/packages/shared/useIntervalFn/demo.vue) • [Docs](https://github.com/antfu/vueuse/blob/master/packages/shared/useIntervalFn/index.md)


<!--FOOTER_ENDS-->