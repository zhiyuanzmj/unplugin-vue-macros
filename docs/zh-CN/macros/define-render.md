# defineRender

<StabilityLevel level="stable" />

使用 `defineRender` 可以直接在 `<script setup>` 中定义渲染函数。

|    特性    |        支持        |
| :--------: | :----------------: |
|   Vue 3    | :white_check_mark: |
|   Nuxt 3   | :white_check_mark: |
|   Vue 2    | :white_check_mark: |
| TypeScript | :white_check_mark: |

## 基本用法

```vue
<script setup lang="tsx">
// 可以直接传递 JSX
defineRender(
  <div>
    <span>Hello</span>
  </div>
)

// 或使用渲染函数
defineRender(() => {
  return (
    <div>
      <h1>Hello World</h1>
    </div>
  )
})
</script>
```
