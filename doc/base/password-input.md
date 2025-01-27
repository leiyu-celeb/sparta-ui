# PasswordInput 密码输入框

### 基础用法

:::demo 简单使用，PasswordInput的宽度默认是100%，如需改变，可加父容器或样式覆盖。
```vue
<template>
  <div class="md-demo-password-input">
    <sp-password-input
      v-model="value1" 
    />
  </div>
</template>
<script>
  export default {
    data() {
      return {
        value1: ''
      }
    },
    watch: {
      value1(val) {
        console.log(val)
      }
    }
  }
</script>
```
:::


### 数字类型

:::demo 简单使用，PasswordInput的宽度默认是100%，如需改变，可加父容器或样式覆盖。
```vue
<template>
  <div class="md-demo-password-input">
    <sp-password-input 
      type="number"
      v-model="value2" 
    />
  </div>
</template>
<script>
  export default {
    data() {
      return {
        value1: ''
      }
    },
    watch: {
      value1(val) {
        console.log(val)
      }
    }
  }
</script>
```
:::



### PasswordInput Attributes

| 参数          | 说明            | 类型            | 可选值                 | 默认值   |
|-------------  |---------------- |---------------- |---------------------- |-------- |
| type         | 类型   | string  | password，number | password
| validateEvent         | 验证   | boolean  | —  |true
| value         | 绑定值           | string / number  | — | — |

### Methods

| 方法名      | 说明          | 参数
|---------- |-------------- | --------------
| focus | 聚焦 | —

<script>
  export default {
    data() {
      return {
        value1: '',
        value2: '',
      }
    },
    watch: {
      value1(val) {
        console.log(val)
      },
      value2(val) {
        console.log(val)
      }
    }
  }
</script>

<style>
.sp-password-input-demo {
}
</style>
