# 语言

```html
<n-space vertical>
  <n-space>
    <n-button @click="locale = null; dateLocale = null">英文</n-button>
    <n-button @click="locale = zhCN; dateLocale = dateZhCN">中文</n-button>
  </n-space>
  <n-config-provider :locale="locale" :date-locale="dateLocale">
    <n-date-picker />
  </n-config-provider>
</n-space>
```

```js
import { defineComponent, ref } from 'vue'
import { zhCN, dateZhCN } from 'naive-ui'

export default defineComponent({
  setup () {
    return {
      zhCN,
      dateZhCN,
      locale: ref(null),
      dateLocale: ref(null)
    }
  }
})
```
