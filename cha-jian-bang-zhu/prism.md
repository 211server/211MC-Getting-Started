# Prism

[Prism](https://github.com/prism/Prism) 插件会自动记录方块和物品变动.

```text
/pr near
```

此命令用于快速查询当前所在坐标周围几格之内的最近变动记录.

```text
/pr lookup {parameters}
```

此命令提供高级查询, 可用参数如下

* `a:(event)` - "Action". `break`, `place`, etc.
* `b:(block id)` - "Block" name. Like "grass".
* `before:(time)` - "Before" time period.
* `c:(cause)` - Non-player causes, i.e. "environment"
* `player:(name)` - "Player" name. May be an offline player.
* `r:(number)` - "Radius" - A distance around you.
* `since:(time)` - "Since" time period.

使用例子:

```text
/pr lookup a:break player:czp3009 since:3d
```

查询玩家 `czp3009` 在过去 `3` 天内 `破坏` 的方块.

