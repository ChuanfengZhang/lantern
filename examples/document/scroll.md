### 实例

::: demo demo

```html
  <div style="width:100%;height:300px">
    <lt-scroll
      @on-scroll="onScroll"
    >
      <p>1.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>2.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>3.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>4.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>6.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>7.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>8.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>9.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
      <br />
      <p>10.测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容测试内容</p>
    </lt-scroll>
  </div>
```

:::

### lt-scroll 参数

| 参数             | 说明                                       | 类型   | 必选 | 默认值 |
| ---------------- | ------------------------------------------ | ------ | ---- | ------ |
| barStyle         | 滚动条配置(通过该对象传递滚动条所有的配置) | Object | 否   | {}     |
| scrollReloadTag  | 滚动条重载标志                             | Number | 否   | null   |
| defaultScrollTop | 滚动条默认高度                             | Number | 否   | null   |
| rightScrollShow | 是否显示右部滚动条                             | Boolean | 否   | true   |
| bottomScrollShow | 是否显示底部滚动条                             | Boolean | 否   | true   |
| scrollToTop | 是否滚动到顶部                             | Number | 否   |    |

#### barStyle 配置说明

参数|说明|类型|必选|默认值
--------|--------|--------|--------|--------
barColor|滚动条的颜色|String|否|'#959595'
trackColor|滚动条轨道的颜色|String|否|'#eee'
barWidth|滚动条的宽度|Number|否|8
barHeight|滚动条的高度|Number|否|8
barOpacityInactive|滚动条的非活动时的透明度|Number|否|0.3
zIndex|滚动条的z-index|String|否|'auto'
wrapWidth|容器的宽度(带单位的字符串如'100%'、'100px')|String|否|'100%'
wrapHeight|容器的高度(带单位的字符串如'100%'、'100px')|String|否|'100%'
autoHide|是否自动隐藏滚动条|Bollen|否|true

::::vuecode::::
<script>
export default {
  methods: {
    onScroll(eve) {
      console.log(eve)
    }
  }
}
</script>
<style lang="less" scoped>

</style>