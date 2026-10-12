<p align="right"><a href="https://github.com/MoonMere/lianliankan-wechat-game"><kbd>English</kbd></a></p>

# 外婆爱游戏

这是一款连连看游戏，以微信小游戏的形式发布。它是我的个人项目，2026 年 7 月到 8 月期间，我指挥 AI 编程工具 Claude Code 把它做了出来。

这款游戏最初是我为外婆做的，名字就是这么来的。到 2026 年 8 月，它已经在微信上线，任何人都可以玩。

<table>
  <tr>
    <td><img src="images/01_board.png" width="200" alt="由动物方块组成的棋盘，其中一个方块被选中了"></td>
    <td><img src="images/02_pause_menu.png" width="200" alt="暂停菜单"></td>
    <td><img src="images/03_auto_reshuffle.png" width="200" alt="一条横幅，提示没有能连的了，棋盘会重新排列"></td>
    <td><img src="images/04_time_up.png" width="200" alt="时间到的界面，上面有一个再试一次的按钮"></td>
  </tr>
  <tr>
    <td align="center">游戏进行中的棋盘</td>
    <td align="center">暂停菜单</td>
    <td align="center">没有能连的了，游戏会自动重新排</td>
    <td align="center">时间到</td>
  </tr>
</table>

## 玩法

- 点击两个相同的动物即可消除。连接它们的线最多拐两个弯。
- 在时间条走完之前清空棋盘。每个新棋盘的限时会根据你玩得快慢来调整。
- “提示”和“重新排一下”免费，不限次数。没有能连的了，游戏也会替你重新排。

游戏里没有广告，也没有需要付费购买的内容。游戏内的文字全部是中文。

## 我是怎么用 AI 做出来的

所有代码都是 Claude Code 写的。游戏使用 TypeScript 和 Cocos Creator 3.8 游戏引擎。我负责决定游戏要做成什么样，过程中随时拍板，还负责测试和发布。

- 一系列 AI 对话先写出详细的计划，并把工作拆成步骤，另一些对话再按这些步骤写出大部分代码。每次对话结束时都会留下一份交接说明，这样下一次对话就能从上次停下的地方接着做。
- 重大决定由我自己做，技术细节和一部分设计上的选择交给 AI。外观方面，AI 先做出三种视觉风格的样稿，由我选定其中一种。
- AI 为游戏逻辑写了自动化测试，还把画面上的改动和设计样稿做了对照。我在自己的手机上测试构建出来的版本，微信的注册和审核也由我自己办理。

## 在微信上

在微信上，这款游戏叫 **外婆爱游戏**。

<img src="images/05_loading_screen.png" width="240" alt="微信的加载画面，显示着游戏名称“外婆爱游戏”">

## 关于这个仓库

这个仓库只存放这份说明和一些截图。四张游戏截图是 2026 年 7 月从微信开发者工具的模拟器里截取的。加载画面是在手机上截取的。

## 致谢

- 动物图标：[Noto Color Emoji](https://github.com/googlefonts/noto-emoji)，Google 出品，Apache License 2.0
- 字体：Noto Serif SC，SIL Open Font License
- 音效：[Kenney](https://kenney.nl)，CC0
