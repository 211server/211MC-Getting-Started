# Essential

[Essential](https://github.com/EssentialsX/Essentials) 是 Minecraft 基础插件, 提供一系列常用命令.

## Home

```text
/sethome
```

在当前坐标创建"家", 若已设置过"家"则会覆盖上一次的设置.

```text
/home
```

传送回此前设置的"家".

## Spawn

```text
/spawn
```

传送至当前世界的出生点.

```text
/firstspawn
```

传送至新玩家第一次进入服务器时的出生点\(若服务器规则未额外说明, 则与 /spawn 传送到的地点一致\).

## Warp

```text
/warp list
```

查看当前服务器所有地标\(由管理员设定\).

```text
/warp {name}
```

传送至某个地标\(可能不在当前世界\).

## TPA

这是玩家间传送的主要方式

```text
/tpa {playerName}
```

请求传送至某个玩家\(必须在线\), 目标玩家会收到一个传送请求.

```text
/tpahere {playerName}
```

请求将某个玩家传送到自己所在的坐标, 目标玩家会收到一个传送请求.

```text
/tpaccept
```

收到传送请求时同意此请求.

```text
/tpdeny
```

收到传送请求时拒绝此请求.

## 杂项

```text
/rtp
```

此命令会将使用者随机传送到某个地点, 可能会传送入岩石/掉入岩浆/被怪物炸死. 若因此造成任何损失, 欢迎多试几次.

```text
/gc
```

查看服务器当前运行状况.

