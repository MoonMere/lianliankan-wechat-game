<details name="lang">
<summary><kbd>中文</kbd></summary>

# 外婆爱游戏

这是一款连连看游戏，以微信小游戏的形式发布。它是我的个人项目，2026 年 7 月到 8 月期间，我指挥 Claude Code 把它做了出来。

这款游戏最初是我为外婆做的，名字就是这么来的。她原来玩的那款连连看广告很多，很容易误点。国内平台上的这类游戏都塞满了广告，随手一点就可能开始下载，甚至付费。我做这个版本就是为了解决这个问题，所以游戏里完全没有广告。到 2026 年 8 月，它已经在微信上线，任何人都可以玩。

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
- 重大决定由我自己做，技术细节和一部分设计上的选择交给 AI。外观方面，AI 先做出三种视觉风格的样稿，由我选定其中一种。我还让“重新排一下”挪到“提示”旁边，点一下就能用。
- 外观改了好几轮才对。选定的风格做出来三版，在我的手机上三次都没通过检查。第三版底部两个按钮明显偏右，可 AI 之前汇报说已经改好了。于是我专门试了试，看一个全新的 AI 对话能不能找出截图和样稿之间的不同。从那以后，检查画面分两步：先让一个全新的对话列出它看到的所有不同，再把每一处都量出来。
- 我定了一条规矩：检查和测试比代码本身更重要。AI 为游戏逻辑写了自动化测试，我在自己的手机上测试构建出来的版本。微信的注册和审核也由我自己办理。
- 上线以后，我发现这个游戏在微信里没法转发给朋友。我想让所有人都能玩、都能转给朋友，所以 0.1.6 版开启了转发，转发卡片的标题“没有广告，不费流量，完全免费的连连看”是我写的。

## 在微信上

想玩的话，在微信里搜“外婆爱游戏”。

<img src="images/05_loading_screen.png" width="240" alt="微信的加载画面，显示着游戏名称“外婆爱游戏”">

## 关于这个仓库

这个仓库只存放这份说明和一些截图。四张游戏截图是 2026 年 7 月从微信开发者工具的模拟器里截取的。加载画面是在手机上截取的。

## 致谢

- 动物图标：[Noto Color Emoji](https://github.com/googlefonts/noto-emoji)，Google 出品，Apache License 2.0
- 字体：Noto Serif SC，SIL Open Font License
- 音效：[Kenney](https://kenney.nl)，CC0

</details>

<details name="lang" open>
<summary><kbd>English</kbd></summary>

# 外婆爱游戏 (Granny Loves Games)

A lianliankan (连连看) tile matching game, released as a WeChat Mini Game. It is a personal project that I built between July and August 2026 by directing Claude Code.

I first made it for my grandmother, which is where the name comes from. The lianliankan app she played was full of ads that were easy to tap by mistake. Games like this on Chinese platforms are packed with ads, and one careless tap can start a download or even a payment. I made this version to fix that, so it has no ads at all. By August 2026, it was live on WeChat for anyone to play.

<table>
  <tr>
    <td><img src="images/01_board.png" width="200" alt="A board of animal tiles with one tile selected"></td>
    <td><img src="images/02_pause_menu.png" width="200" alt="The pause menu"></td>
    <td><img src="images/03_auto_reshuffle.png" width="200" alt="A banner saying there are no moves left and the board will be reshuffled"></td>
    <td><img src="images/04_time_up.png" width="200" alt="The time up screen with a button to try again"></td>
  </tr>
  <tr>
    <td align="center">A board in play</td>
    <td align="center">Pause menu</td>
    <td align="center">No moves left, so the game reshuffles</td>
    <td align="center">Time is up</td>
  </tr>
</table>

## How to play

- Tap two matching animals to clear them. The line joining them can turn at most twice.
- Clear the board before the time bar runs out. The time limit for each new board adapts to how fast you play.
- 提示 (Hint) and 重新排一下 (Reshuffle) are free and unlimited, and the game reshuffles for you when no moves are left.

The game has no ads and nothing to buy. All text in the game is in Chinese.

## How I made it with AI

Claude Code wrote all of the code. The game uses TypeScript and the Cocos Creator 3.8 game engine. My part was deciding what the game should be, making the calls along the way, testing it and releasing it.

- A series of AI conversations wrote a detailed plan and broke the work into steps. Other conversations wrote most of the code from those steps. Each conversation ended with a handoff note, so the next one could carry on where it stopped.
- I made the big decisions myself and left technical details and some design choices to the AI. For the look, the AI mocked up three visual styles and I picked one. I also asked for 重新排一下 (Reshuffle) to sit next to 提示 (Hint), so it takes one tap.
- Getting the look right took several rounds. Three builds of the chosen style failed my checks on my phone. In the third, the two bottom buttons sat clearly right of centre, although the AI had reported them as fixed. I then tested whether a fresh AI conversation could spot the differences between a screenshot and the mockup. From then on, every visual check had two steps: a fresh conversation lists every difference it can see, and then each one is measured.
- I set the rule that checks and tests count for more than the code itself. The AI wrote automated tests for the game logic, and I tested builds on my own phone. I also handled the WeChat registration and review myself.
- After launch, I found the game couldn't be forwarded to friends in WeChat. I wanted anyone to be able to play it and pass it on, so version 0.1.6 turned sharing on, with a share card title I wrote: 没有广告，不费流量，完全免费的连连看 ('No ads, no data costs, completely free lianliankan').

## On WeChat

To play it, search for 外婆爱游戏 in WeChat.

<img src="images/05_loading_screen.png" width="240" alt="The WeChat loading screen showing the game name 外婆爱游戏">

## About this repository

This repository only holds this description and some screenshots. The four game screenshots come from the WeChat developer tools simulator in July 2026. The loading screen was captured on a phone.

## Credits

- Animal icons: [Noto Color Emoji](https://github.com/googlefonts/noto-emoji) by Google, Apache License 2.0
- Font: Noto Serif SC, SIL Open Font License
- Sound effects: [Kenney](https://kenney.nl), CC0

</details>
