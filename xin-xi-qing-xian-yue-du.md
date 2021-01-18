# 信息（请先阅读）

网站和 FAQ: [https://kubejs.latvian.dev/](https://kubejs.latvian.dev/)

Discord: [https://discord.gg/bPFfH6P](https://discord.gg/bPFfH6P)

Forge 下载: [https://www.curseforge.com/minecraft/mc-mods/kubejs](https://www.curseforge.com/minecraft/mc-mods/kubejs)

Forge GitHub+Issues Tracker: [https://github.com/KubeJS-Mods/KubeJS](https://github.com/KubeJS-Mods/KubeJS)

Fabric 下载: [https://www.curseforge.com/minecraft/mc-mods/kubejs-fabric](https://www.curseforge.com/minecraft/mc-mods/kubejs-fabric)

Fabric GitHub+Issues Tracker: [https://github.com/KubeJS-Mods/KubeJS-Fabric](https://github.com/KubeJS-Mods/KubeJS-Fabric)

{% hint style="warning" %}
1.12 版本已停止支持, 只有1.15及以上仍在支持!
{% endhint %}

### 如何阅读变量和函数

| 格式 | 使用例 | 附加信息 |
| :--- | :--- | :--- |
| variableName | var x = event.variableName event.variableName = 10 | 一个简单的变量，可以被读取和更改 |
| functionName\(\) | event.functionName\(\) | 没有参数的函数，可以被调用 |
| functionName\(int x, String y\) | event.functionName\(\) | 有指定类型的参数的函数（即使JS没有函数类型）也可以被调用 |
| _variableName_ | var x = event.variableName | 只能被读取而不能被更改的变量 |
| _variableName_ | event.variableName = 10 | 只能被改变而不能被读取的变量 |

