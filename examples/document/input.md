## 输入框input
表单组件

### 基础用法
:::demo demo
```html
  <div>
    <LtInput type="input" v-model="test" />
  </div>
```
:::

### 文本域

用于输入多行文字，设置`type`为`textarea`，通过设置`rows`控制默认行数

::: demo demo
```html
  <div style="float: left; width: 49%">
    <lt-input type="textarea" rows="3"></lt-input>
  </div>
  <div style="float: right; width: 49%">
    <lt-input type="textarea" :maxlength="100" rows="6"></lt-input>
  </div>
```
:::

### 禁用状态

通过添加`disabled`属性可设置为不可用状态。

::: demo demo
```html
  <div style="width: 300px">
    <lt-input type="textarea" disabled></lt-input>
  </div>
```
:::

### Attributes

参数|说明|类型|可选值|默认值
--------|--------|--------|--------|--------
type|输入框类型|String|text/textarea|text
value|绑定值|String|-|-
placeholder|输入框占位|String|-|请输入
maxlength|最大输入长度|String/Number|-|-
disabled|禁用输入框|Boolean|true/false|false
readonly|只读|Boolean|true/false|false
rows|行数（只有在type为textarea才生效）|String , Number|-|4

### Events

事件名|说明|回调参数
--------|--------|--------
blur|input失去焦点触发|event
focus|input得到焦点触发|event
change|input值更改触发|value: input的value值

::::vuecode::::
<script>
export default {
  data () {
    return {
      test: ''
    }
  },
  watch: {
    test: function () {
      console.log(this.test)
    }
  }
}
</script>