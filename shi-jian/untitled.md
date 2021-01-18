# 全部事件列表

全部事件的列表。可能不是所有的事件都被列在这里，但这个清单会被频繁更新。

点击事件ID以查看它的类和信息，字段和方法

种类描述：

* 启动时：将脚本文件放置在 `kubejs/startup_scripts` 文件夹。
* 服务端：将脚本文件放置在 `kubejs/server_scripts` 文件夹。会在输入`/reload`指令的时候被重载。
* 服务端启动时：与服务器相同，且事件会在服务器加载的时候被触发至少一次。
* 客户端：将脚本文件放置在 `kubejs/client_scripts` 文件夹。目前只有在你安装了KubeJS UI，并在菜单中按下`Ctrl+F5`时才会被重载。
* 客户端启动时：与客户端相同，且事件会在服务器加载的时候被触发至少一次。

| ID | 可取消 | 类型 | 是否在Fabric上可用 |
| :--- | :--- | :--- | :--- |
| [init](https://mods.latvian.dev/books/kubejs/page/eventjs) | No | Startup | Yes |
| [postinit](https://mods.latvian.dev/books/kubejs/page/eventjs) | No | Startup | Yes |
| [loaded](https://mods.latvian.dev/books/kubejs/page/eventjs) | No | Startup | Yes |
| command.registry | No | Server Startup | Yes \(从 3. 1 版本起\) |
| [command.run](https://mods.latvian.dev/books/kubejs/page/commandeventjs) | Yes | Server | Yes \(从 3. 1 版本起\) |
| [client.init](https://mods.latvian.dev/books/kubejs/page/eventjs) | No | Client Startup | Yes |
| client.debug\_info.left | No | Client | Yes |
| client.debug\_info.right | No | Client | Yes |
| client.logged\_in | No | Client | Yes \(从 3. 1 版本起\) |
| client.logged\_out | No | Client | Yes \(从 3. 1 版本起\) |
| client.tick | No | Client | Yes |
| client.item\_tooltip | No | Client | Yes |
| server.load | No | Server Startup | Yes \(从 3. 1 版本起\) |
| server.unload | No | Server | Yes \(从 3. 1 版本起\) |
| server.tick | No | Server | Yes |
| server.datapack.first | No | Server Startup | Yes |
| server.datapack.last | No | Server Startup | Yes |
| [recipes](https://mods.latvian.dev/books/kubejs/page/recipeeventjs) | No | Server Startup | Yes |
| world.load | No | Server | Yes |
| world.unload | No | Server | Yes |
| world.tick | No | Server | Yes |
| world.explosion.pre | Yes | Server | Yes \(从 3. 1 版本起\) |
| world.explosion.post | No | Server | Yes \(从 3. 1 版本起\)\) |
| player.logged\_in | No | Server | Yes \(从 3. 1 版本起\) |
| player.logged\_out | No | Server | Yes \(从 3. 1 版本起\) |
| player.tick | No | Server | Yes \(从 3. 1 版本起\) |
| player.data\_from\_server. | Yes | Client | Yes \(从 3. 1 版本起\) |
| player.data\_from\_client. | Yes | Server | Yes \(从 3. 1 版本起\) |
| player.chat | Yes | Server | Yes \(从 3. 1 版本起\) |
| player.advancement | No | Server | Yes \(从 3. 1 版本起\) |
| player.inventory.opened | No | Server | Yes \(从 3. 1 版本起\) |
| player.inventory.closed | No | Server | Yes \(从 3. 1 版本起\) |
| player.inventory.changed | No | Server | Yes \(从 3. 1 版本起\) |
| player.chest.opened | No | Server | Yes \(从 3. 1 版本起\) |
| player.chest.closed | No | Server | Yes \(从 3. 1 版本起\) |
| entity.death | Yes | Server | Yes \(从 3. 1 版本起\) |
| entity.attack | Yes | Server | Yes \(从 3. 1 版本起\) |
| entity.drops | Yes | Server | No |
| entity.check\_spawn | Yes | Server | No |
| entity.spawned | Yes | Server | Yes \(从 3. 1 版本起\) |
| block.registry | No | Startup | Yes |
| block.missing\_mappings | No | Server Startup | No |
| [block.tags](https://mods.latvian.dev/books/kubejs/page/tageventjs) | No | Server Startup | Yes |
| block.right\_click | Yes | Server | Yes |
| block.left\_click | Yes | Server | Yes |
| block.place | Yes | Server | Yes \(从 3. 1 版本起\) |
| block.break | Yes | Server | Yes \(从 3. 1 版本起\) |
| block.drops | No | Server | No |
| item.registry | No | Startup | Yes |
| item.missing\_mappings | No | Server Startup | No |
| [item.tags](https://mods.latvian.dev/books/kubejs/page/tageventjs) | No | Server Startup | Yes |
| item.right\_click | Yes | Server | Yes |
| item.right\_click\_empty | No | Server | Yes |
| item.left\_click | No | Server | Yes |
| item.entity\_interact | Yes | Server | Yes \(从 3. 1 版本起\) |
| item.pickup | Yes | Server | Yes |
| item.toss | Yes | Server | Yes |
| item.crafted | No | Server | Yes \(从 3. 1 版本起\) |
| item.smelted | No | Server | Yes |
| [fluid.tags](https://mods.latvian.dev/books/kubejs/page/tageventjs) | No | Server Startup | Yes |
| [entity\_type.tags](https://mods.latvian.dev/books/kubejs/page/tageventjs) | No | Server | Yes |
| [worldgen.add](https://mods.latvian.dev/books/kubejs/page/worldgenaddeventjs) | No | Startup | Yes |
| [worldgen.remove](https://mods.latvian.dev/books/kubejs/page/worldgenremoveeventjs) | No | Startup | Yes |

