---
category: UI Bars
type: UI Bars
chinese: 标签栏
english: TabBar
---

位于 app 底部，方便用户在不同功能模块之间进行快速切换。

### 规则
- 用作 app 的一级分类，数量控制在 3-5 个之间。
- 即使某个 Tab 不可用，也不要禁用或者移除该 Tab。
- 使用 Badge 进行提示，足不出户也能知道有内容更新。

## API

### TabBar

| 参数             | 说明                                         | 类型     | 默认值        |
|------------------|----------------------------------------------|----------|---------------|
| barTintColor        | tabbar 背景色                     | String   | `white`            |
| tintColor         | 选中的字体颜色                               | String | `#108ee9`         |
| unselectedTintColor       | 未选中的字体颜色  | String | '#888'           |
| prefixCls(`web only`) | 样式前缀  | String   | 'am-tabbar'      |


### TabBar.Item

| 参数 | 说明             | 类型                    | 默认值 |
|------|------------------|-------------------------|--------|
| badge  | 徽标数  | Number \ String           | 无     |
| onPress  | bar 点击触发，需要自己改变组件 state & selecte={true} | Function | `(){}`     |
| selected  | 是否选中 | Boolean | false     |
| icon  | 默认展示图片 | Image Source(rn) \ {uri: String} (web) |      |
| selectedIcon  |  选中后的展示图片 | Image Source(rn) \ {uri: String} (web) |      |
| title  |  标题文字 | String |      |
