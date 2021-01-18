# TagEventJS

{% hint style="info" %}
加载标签集合以使用脚本对其进行修改时此事件会被触发。 即可以为项目，块，流体和实体类型添加和删除标签。
{% endhint %}

### 父类

[EventJS](eventjs.md)

### 是否可取消

否

### 变量与函数

| 名称 | 类型 | 信息 |
| :--- | :--- | :--- |
| type | String | 标签列表种类。 |
| get\(String tag\) | TagWrapper | 返回特定的标签容器，可用于向其添加或删除对象。 标签参数可以类似于`“forge:ingots/copper”`。 如果标签不存在，它将创建一个新标签。 |
|  add\([String](https://mods.latvian.dev/books/kubejs/page/string) tag, [String](https://mods.latvian.dev/books/kubejs/page/string)\[\]/Regex ids\) | TagWrapper | `event.get(tag).add(ids)`的便捷写法 |
|  remove\([String](https://mods.latvian.dev/books/kubejs/page/string) tag, [String](https://mods.latvian.dev/books/kubejs/page/string)\[\]/Regex ids\) | TagWrapper | `event.get(tag).remove(ids)`的便捷写法 |
|  removeAll\([String](https://mods.latvian.dev/books/kubejs/page/string) tag\) | TagWrapper | `event.get(tag).removeAll()`的便捷写法 |

## TagWapper类

### 变量与函数

| 名称 | 类型 | 信息 |
| :--- | :--- | :--- |
|  add\([String](https://mods.latvian.dev/books/kubejs/page/string)\[\]/Regex ids\) | TagWrapper \(itself\) | 将对象添加到此标签。 如果字符串以`＃`开头，则它将添加第二个标签中的所有对象。 它可以是单个字符串，正则表达式`(/regex/flags)`或二者之一的数组。 |
|  remove\([String](https://mods.latvian.dev/books/kubejs/page/string)\[\]/Regex ids\) | TagWrapper \(itself\) | 从标签中删除一个对象，其作用与`add()`相同。 |
| removeAll\(\) | TagWrapper \(itself\) | 从标签中删除所有对象。 |

### 示例

```javascript
// 监听任务标签事件
onEvent('item.tags', event => {
  // 获取 #forge:cobblestone 标签列表，并向其中加入 minecraft:diamond_ore
  event.add('forge:cobblestone', 'minecraft:diamond_ore')
  
  // 获取 #forge:cobblestone 标签列表，并将 minecraft:mossy_cobblestone 从中移除
  event.remove('forge:cobblestone', 'minecraft:mossy_cobblestone')
  
  // 获取 #forge:ingots/copper 标签中的所有对象并全部移除
  event.removeAll('forge:ingots/copper')
})
```

{% hint style="danger" %}
配方使用物品标签，而不是方块标签或流体标签，即使代表那些标签的物品是方块也是如此。 就像`minecraft:cobblestone`一样，即使它是一个方块，它仍将是配方的物品标签。
{% endhint %}

{% hint style="info" %}
`block.tags`事件用于向方块类型添加标签，其工作方式相同。 如果从侧面看启用了F3的方块，则可以找到现有的方块标签。 这些大多仅出于技术原因而使用，并且如上所述，如果将其用于配方/物品栏，则即使是方块也要使用`item.tags`。
{% endhint %}

