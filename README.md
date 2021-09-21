# Bilibili-Advanced-Danmaku-Sender
一个将 lrc 歌词文件自动转换为 B 站高级弹幕并发送的小工具

## 效果
查看我创建的 [弹幕姬作品合集](https://space.bilibili.com/143403774/favlist?fid=1350008174) 收藏夹

## 使用
本文档只会讲述如何获取 Cookies。

1. 打开你要发送弹幕的视频
2. 按下 F12 打开开发者工具，切换至`Network`选项卡
3. 刷新当前页面
4. 在请求列表中找到有 BV 号的列表项，点击打开
5. 右边窗口选择`Headers`选项卡，下拉，在`Request Headers`中找到`cookie`，全部复制并粘贴至弹幕姬

## DanCode（开发中）
DanCode 是一个可用于自定义弹幕参数的文本参数。合理使用 DanCode 可以增强高级弹幕的表现效果。

DanCode 灵感来自 BBCode。

### `[pos][/pos]`
该 DanCode 支持自定义高级弹幕位置，包括起始位置和终止位置。

以下是使用示例：

```bbcode
[pos=x,y]Danmaku[/pos]
[pos=起始x,起始y,结束x,结束y]Danmaku[/pos]
Dan[pos=x,y]maku[/pos]
```

请注意，虽然您可以使用示例的第三种方式，但 DanCode 外两边的内容会被直接合在一起，故请留下适当的空格。

### 预计开发的 DanCode
* [color][/color]
* [delay][/delay]
* [time][/time]
* [loop][/loop]
