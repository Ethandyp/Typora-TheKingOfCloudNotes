## typora软件使用(包含markdown语法)

![image-20211204152321879](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211204152321879.png)

## 目录

[TOC]

## 1、什么是markdown

![image-20211125161231337](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125161231337.png)

### 1.Markdown 是什么

> Markdown 是一种**轻量级标记语言**，创始人为约翰·格鲁伯（John Gruber）。它允许人们「使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档 」—— 维基百科

如果你看不懂以上维基百科对 Markdown 的定义，就当这段掐了没播。约翰·格鲁伯自己对Markdown的描述的重点也在于 **「easy-to-read，easy-to-write」。**

### 2.那么到底 easy 在哪里呢

虽然称作 「标记语言」，但简单理解 Markdown 就是在文本前增加符号来表示文本格式。你不需要关心标题多大号，列表缩进多少，是否对齐，只要使用了同一种符号标记，Markdown 已经帮你做好了排版。

无图无真相：
![image-20211125161126505](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125161126505.png)

### 3.Markdown 的好处

1. **编辑，不用操心排版**你只需要把注意力放在内容上。笔者在用 Markdown 之前，打开word 先想想，标题用啥字体呢，几号字呢？不知不觉我的意志力就被消耗了。**实际上所谓排版，不就是作者的思路以及内容的层级和结构么**，在学会使用 Markdown 之后，几个简单的符号就把这些事儿搞定，样式还特别工整精美。
2. **修改，不用担心排版**想想那些你在同事之间改来改去的 word 文档吧，如果哪位童鞋从外部粘贴了一段带格式的文字，那么你再次打开文档时会发现整个人都不好了：格式被改的乱七八糟，还要重新调整。如果用 Markdown 群组笔记 ，想改哪里改哪里，根本不用担心格式，改完评论里直接 @TA，多轻松！

一句话来说，Markdown 是用最简单的方式，零排版成本，写出布局工整、阅读舒适的笔记。**减少干扰，降低成本，提高效率**，不管在什么设备上，看起来都是一个工整的样子。不仅自己阅读爽，分享给朋友也有面儿不是~

### 4.哪些牛人都在用

* 阳志平在 2012 年就发博客推崇了一下 Markdown，但那篇文章虽解读深刻，但也略显极客，**把Markdown 不仅能排版，能做流程图，还支持数学公式的特性**介绍了一遍，**连科技论文都要选择 Markdown** 都涉猎到了。有兴趣阅读的童鞋可[点击这里](http://www.yangzhiping.com/tech/r-markdown-knitr.html) （**注意：这个链接目前打不开了。。**）查看。

* 很多在线博客和内容社区都提供 Markdown 编辑器，不仅在阅读上带来了舒适、统一、美好的体验，每一个参与写作的人，也能够毫不费力地写出排版整齐的文章来。
* 我遇到的很多运维大佬也是采用这个typora来作为课件使用来着的！



**来个小技巧**：

不管我再怎么说 Markdown 的语法记忆负担小、简单，在最初你都会有点儿晕。在这里给大家分享个小技巧：

1. 最初只需要记住 `# 标题一`、`### 标题二`、`1. 第一点`、`* 这一点`，用这几个写写日志、需求文档、小文章，排版上足够了；
2. 逐渐的你发现有些文字需要重点指出，那么还可以使用 `**加粗**`、`*斜体*` 来对文字做重点说明；
3. 如果你是名程序员，那么可以用 ```` `把代码块包起来，**渲染后可以关键字高亮**（666），用 `>` 可以做引用 ；

### 5.Markdown 格式标记符号说明(&Typora常用快捷键)

#### 1.标题

* **Typora快捷键：**`Ctrl/Cmd + 数字` (数字可以是1到6分别代表不同级标题)

- 提升标题级别：`ctrl +`

- 降低标题级别：`ctrl -`

* **markdown语法：**

在行首插入 1 到 6个#，分别表示标题 1 到标题 6

```
# 这是标题1
### 这是标题1
###### 这是标题6
```

点击保存后的效果：
![image-20210130233909849](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130233909849.png)

#### 2. 有序列表

- **Typora快捷键：**`ctrl shift [`

- **markdown语法：**

在行首增加 `1.`、`2.`、`3.`，即数字和英文句点, 注意句点与文字中间有空格。**不要求数字一定要连续，可以都是`1. `**

```
1. 有序列表
1. 有序列表
4. 有序列表
```

点击保存后的效果：

1. 有序列表
2. 有序列表
3. 有序列表



**备注：**

直接在文字前面按回车后，是可以自动排序的；（无序列表也是一样的）

#### 3. 无序列表

- **Typora快捷键：**`ctrl shift ]`

- **markdown语法：**

在行首增加 `*` 或 `- `或`+`与文字之间有空格

```
* 无序列表
- 无序列表
+ 无序列表
```

点击保存后的效果：

- 无序列表
- 无序列表

#### 4. 插入图片

- **Typora快捷键：**`ctrl+shift+i`

- **markdown语法：**

可直接粘贴图片，或将图片文件拖动到光标处。

也可以使用标准的Markdown语法，如：
` ![](http://cdn.wiz.cn/wp-content/uploads/2015/06/wiz_logo.png)`

![image-20210130233504646](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130233504646.png)

#### 5. 插入链接

- **Typora快捷键：**`Ctrl/Cmd + K`

- **markdown语法：**

`[描述](链接地址) ，例如：[为知笔记](http://www.wiz.cn)，注意要使用英文符号`

点击保存后的效果：
[为知笔记](http://www.wiz.cn/)

#### 6. 粗体、斜体、删除线、下划线

- **Typora快捷键：**

  - 加粗： `Ctrl/Cmd + B`

  - 斜体：`ctrl + i`

  - 删除线：`alt+shift+5`
  - 下划线：`ctrl + u`

- **markdown语法：**

粗体：在文字前后添加 `**` (注意符号与文字间不要有空格）
斜体：在文字前后添加 `*`
删除线：在文字前后添加 `~~`

下划线：`ctrl + u`

1. `**粗体**`
2. `*斜体*`
3. `~~删除线~~`
4. <u>下划线</u>

保存后的效果：

**粗体**
*斜体*
~~删除线~~

<u>下划线</u>

#### 7. 引用

- **Typora快捷键：**

- **markdown语法：**

在文字前 添加 `>`

点击保存后的效果：

> 如果你无法简洁的表达你的想法，那只说明你还不够了解它。 -- 阿尔伯特·爱因斯坦

#### 8. 表格

- **Typora快捷键：**插入表格：`ctrl T`
  * 下方插入行：`ctrl enter`
  * 上移该行：`alt 向上箭头`
  * 下移该行：`alt 向下箭头`
  * 左移该行：`alt 向左箭头`
  * 右移该行：`alt 向右箭头`

- **markdown语法：**

1. `| 为知笔记|更新 | 版本 |`
2. `|------------|-----------|--------|`
3. `| WizNote | Markdown| Latest |`

点击保存后的效果：

| 为知笔记 | 更新     | 版本   |
| -------- | -------- | ------ |
| WizNote  | Markdown | Latest |

#### 9. 代码

- **Typora快捷键：**如下。

- **markdown语法：**

先输入 三个反单引号：```，然后直接回车，就会弹出代码框了：

```
int i = 0; i = 1; 
for (int i = 0; i < 100; i++)
{
      printf("hello markdown!\n");
}
```

如果需要指定语言， 在开头的3个反向单引号 后紧跟具体语言即可，如: ```bash  **（注意，这个功能很实用！！！）**

```bash
yum install -y sl
```



或者按`ctrl shift K`即可弹出代码框：

```
啦啦啦
```

#### 10. 目录

在任何你想要展示Markdown 笔记目录的地方，添加 `[TOC] `， 在阅读模式下，标题1~6样式的内容会被提取出来作为目录，相当于大纲功能。

例如：
![image-20210130234016969](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130234016969.png)

#### 11.首行缩进

```
在需要缩进的地方加如下2个字符：
&emsp;&emsp;
```

&emsp;&emsp; 爱一个人真的很痛！

真的很难忘记你。

#### 12.分割线

连续输入3个+号，回车即可插入一个分割线：

**效果如下：**

+++

#### 13.代办清单

```
-[x] 已完成项目1
-[x] 已完成项目2

- [ ] 代办项目1
- [ ] 代办项目2
```

**效果如下：**

- [x] 已完成项目1

- [x] 已完成项目2

    

- [ ] 代办项目1

- [ ] 代办项目2

#### 14.Typora其他快捷键

1. 插入公式块：`ctrl shift M`
2. 清除样式：`ctrl \`
3. 粘贴为纯文本：`ctrl shift v`
4. 撤销： Ctrl/Cmd + Z
5. 显示/隐藏侧边栏：`ctrl + shift + L`，等价于`ctrl + shift + 1`
6. 搜索：`ctrl+f`
7. 源代码模式：`ctrl+/`（很少使用）
8. 切换全屏：`F11` #再次按F11就可以退出全屏模式了；
9. 放大、缩小、还原：
   * 放大：`ctrl + shift + =`
   * 缩小：`ctrl + shift + -`
   * 还原：`ctrl + shift + =9`
10. 应用内窗口切换：`ctrl + Tab`
11. 开发者工具：`shift + F12`
12. 表情和符号：`windows + 句号`



* **建议平常写作时，使用快捷键，使用快捷键，使用快捷键**，语法了解即可。

* 注意：Typora快捷键可以在菜单里查看：
  ![image-20210130234039447](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130234039447.png)

## 2、什么是typora及其常用配置

写Markdown费事？Typora让你像写word一样行云流水，所见即所得。
![image-20211125161540027](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125161540027.png)

### 1.什么是typora

* Typora删除了预览窗口，以及所有其他不必要的干扰。**取而代之的是实时预览。**
* Markdown的语法因不同的解析器或编辑器而异，Typora使用的是[GitHub Flavored Markdown](https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)。

![image-20211127075142961](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211127075142961.png)

![image-20211127075208634](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211127075208634.png)

![image-20211127075229699](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211127075229699.png)

![image-20211127075256876](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211127075256876.png)

### 2.下载

[Typora下载](https://www.typora.io/#download)

![image-20211125161712909](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125161712909.png)

### 3.优点

> Typora 最舒服的是所见即所得的排版，以及实时渲染带来的沉浸式写作体验，非常舒服。

用官方的话描述：

> Typora 提供同时读写的无缝体验，删除了预览窗口、模式切换器、markdown 源代码的语法符号以及所有其他不必要的干扰。
>
> 相反，提供了真正的实时预览功能，可帮助您专注于内容本身。

#### :round_pushpin: 所见即所得

`这个功能贼好用，自从使用这个功能后，其他的2边编写方式都是垃圾哈哈……`

通常 MD 编辑器，是左边编辑，右边预览，而typora是直接你写啥直接渲染，不搞双栏。

从现在（2021年）的视角来看，这种所见即所得，即使放到现在，也没有能打的对手，更不用说在当时，有多前卫了。

不用传统的双栏模式，更符合编写习惯。

![](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/jjygysgyc.gif)

#### :round_pushpin: 足够开放

相比众多 Markdown 编辑器，例如 MWeb，Bear ，Typora 的主题允许自行定义，只要你懂点 CSS

如下是我基于少数派的主题改过的 Typora 个人主题，和公众号的排版保质一致。

![image-20211202103600644](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202103600644.png)

#### :round_pushpin: 足够简单

Typora 对内容不过多的干预，不需要注册帐号，数据全部存在本地，没有同步机制（在我看来，这算优点）

#### :round_pushpin: 图床支持

可对接 iPic、uPic 和 PicGo 等知名图床工具，而且还支持 Custom Comand ，这点对于集成更多第三方插件提供了便利！

![image-20211202103731559](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202103731559.png)

#### :round_pushpin: 版本管理

记得有一次，我在写一篇一万多字的文章时（是真的一万多字，不包含代码），不小心删除了文章内容，无论怎么 Command + z 回退都没用，最后在版本管理这边找到了历史版本，有惊无险。

版本管理，对于文章来说，平时可能用不太着，但要是碰到特殊情况，它就显得非常非常重要。(windows软件貌似没找到这个功能……)

![image-20211202103909465](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202103909465.png)

#### :round_pushpin: 新版本更新了什么

那么 1.0 的这个付费版本，到底更新了什么史诗级的新功能呢？能让作者将其做为第一个付费版本发布？

我去 CHANGELOG 上瞄了一眼，"平平无奇" 得让我有点不敢相信这就是付费版本。

![image-20211202104120014](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202104120014.png)

总结起来，就两点：

1. 支持 ARM 版本 Windows 和 Linux

2. 在编辑数学公式时提供开关来支持是否开启使用 \ 来换行

![image-20211202104150618](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202104150618.png)

新版本有 15 天的试用期，最后一个免费版本是 0.11.18，可以点这里下载 （失效了的话可以加我微信获取！）

```
Linux：https://wwe.lanzoui.com/igFedwzagle
MacOS：https://wwe.lanzoui.com/ip9ijwzagpi
Windows：https://wwe.lanzoui.com/i8PP3wzahrg
```

不过作者在 What's New? 上特别感谢了这么多年来一直使用 Typora 并且帮助 Typora 变得更好的测试者

![image-20211202104217431](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202104217431.png)



而最值得一提的，可能很多人还不知道，其实 Typora 是一款国人开发的软件。

作者是 Abner Lee，在互联网上没有太多作者的介绍，我在知乎上有找到作者的帐号，不过动态非常少，唯一和 Typora 相关的动态是下面这个回答。

![image-20211202104259011](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202104259011.png)

可见作者一直在用心做产品，把产品做好了，就不需要太多的营销手段， Typora 到今天能如此成功，真的是依靠口口相传的口碑。

**最重要的是，作者能坚持 6 年用爱发电，就凭这个，即使 1.0 版本并没有太多亮眼的新特性，我也愿意为它付费！**

![image-20211202104315275](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202104315275.png)

#### :round_pushpin: typora收费情况

在本地使用最多的就是Typora这款软件，之前一直是免费测试版本，最近终于发布了正式版本，下面是明哥对正式版本的分享，致热爱创作或分享的我们。

在 2021.11月23日，Typora 正式发布 1.0 版本，进入了付费时代。

1.0 版本是一次性付费而非订阅的，只要支付人民币 89 元，可以在 3 台设备里使用。

![image-20211202103028083](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202103028083.png)

有的人，可能会说：辣鸡，我用了这么多年，都用习惯了，终于要开割了吗？

其实不然，Typora 一直没有开源，更没有承诺过终身免费，因此对于收费这件事来说，虽说突然，但却也一点不意外。

### 4、缺点

#### 📍 打开大文件时会卡死

2021年12月7日14:35:00update

希望typora的后续版本打开大文件渲染，并且不卡死（现在 typora 打开几万字的 markdown 经常卡死）；一般应该不会怎么超过10w字的吧，一个m

![image-20211207144224677](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207144224677.png)

![image-20211207145754727](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207145754727.png)



- 哈哈：打开有点慢，但还是可以接受的，几乎无感知，除非文档内容很多的吧……

![image-20211207150428691](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207150428691.png)

#### 📍 不支持自己的图床、云端同步

2021年12月7日14:34:22Update

其实 Typora 的核心卖点就是沉浸式的输入体验，其它很多，比如图床、云端同步都没有，需要自己去弄，并且现在其他 Markdown 编辑器的编辑体验其实也不差了。

#### 📍 typora画类图好像不太优秀哈哈

![image-20211207150205426](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207150205426.png)

### 5、typora图标(666)

typora图标(typora真的666啊)，可使用快捷键`win + 。`来快速打开。

#### 1.people

```
😄 :smile:	|😆 :laughing:	 
😊 :blush:	😃 :smiley:	☺️ :relaxed:
😏 :smirk:	😍 :heart_eyes:	😘 :kissing_heart:
😚 :kissing_closed_eyes:	😳 :flushed:	😌 :relieved:
😆 :satisfied:	😁 :grin:	😉 :wink:
😜 :stuck_out_tongue_winking_eye:	😝 :stuck_out_tongue_closed_eyes:	😀 :grinning:
😗 :kissing:	😙 :kissing_smiling_eyes:	😛 :stuck_out_tongue:
😴 :sleeping:	😟 :worried:	😦 :frowning:
😧 :anguished:	😮 :open_mouth:	😬 :grimacing:
😕 :confused:	😯 :hushed:	😑 :expressionless:
😒 :unamused:	😅 :sweat_smile:	😓 :sweat:
😥 :disappointed_relieved:	😩 :weary:	😔 :pensive:
😞 :disappointed:	😖 :confounded:	😨 :fearful:
😰 :cold_sweat:	😣 :persevere:	😢 :cry:
😭 :sob:	😂 :joy:	😲 :astonished:
😱 :scream:	 	😫 :tired_face:
😠 :angry:	😡 :rage:	😤 :triumph:
😪 :sleepy:	😋 :yum:	😷 :mask:
😎 :sunglasses:	😵 :dizzy_face:	👿 :imp:
😈 :smiling_imp:	😐 :neutral_face:	😶 :no_mouth:
😇 :innocent:	👽 :alien:	💛 :yellow_heart:
💙 :blue_heart:	💜 :purple_heart:	❤️ :heart:
💚 :green_heart:	💔 :broken_heart:	💓 :heartbeat:
💗 :heartpulse:	💕 :two_hearts:	💞 :revolving_hearts:
💘 :cupid:	💖 :sparkling_heart:	✨ :sparkles:
⭐️ :star:	🌟 :star2:	💫 :dizzy:
💥 :boom:	💥 :collision:	💢 :anger:
❗️ :exclamation:	❓ :question:	❕ :grey_exclamation:
❔ :grey_question:	💤 :zzz:	💨 :dash:
💦 :sweat_drops:	🎶 :notes:	🎵 :musical_note:
🔥 :fire:	💩 :hankey:	💩 :poop:
💩 :shit:	👍 :+1:	👍 :thumbsup:
👎 :-1:	👎 :thumbsdown:	👌 :ok_hand:
👊 :punch:	👊 :facepunch:	✊ :fist:
✌️ :v:	👋 :wave:	✋ :hand:
✋ :raised_hand:	👐 :open_hands:	☝️ :point_up:
👇 :point_down:	👈 :point_left:	👉 :point_right:
🙌 :raised_hands:	🙏 :pray:	👆 :point_up_2:
👏 :clap:	💪 :muscle:	🤘 :metal:
🖕 :fu:	🚶 :walking:	🏃 :runner:
🏃 :running:	👫 :couple:	👪 :family:
👬 :two_men_holding_hands:	👭 :two_women_holding_hands:	💃 :dancer:
👯 :dancers:	🙆 :ok_woman:	🙅 :no_good:
💁 :information_desk_person:	🙋 :raising_hand:	👰 :bride_with_veil:
🙎 :person_with_pouting_face:	🙍 :person_frowning:	🙇 :bow:
:couplekiss: :couplekiss:	💑 :couple_with_heart:	💆 :massage:
💇 :haircut:	💅 :nail_care:	👦 :boy:
👧 :girl:	👩 :woman:	👨 :man:
👶 :baby:	👵 :older_woman:	👴 :older_man:
👱 :person_with_blond_hair:	👲 :man_with_gua_pi_mao:	👳 :man_with_turban:
👷 :construction_worker:	👮 :cop:	👼 :angel:
👸 :princess:	😺 :smiley_cat:	😸 :smile_cat:
😻 :heart_eyes_cat:	😽 :kissing_cat:	😼 :smirk_cat:
🙀 :scream_cat:	😿 :crying_cat_face:	😹 :joy_cat:
😾 :pouting_cat:	👹 :japanese_ogre:	👺 :japanese_goblin:
🙈 :see_no_evil:	🙉 :hear_no_evil:	🙊 :speak_no_evil:
💂 :guardsman:	💀 :skull:	🐾 :feet:
👄 :lips:	💋 :kiss:	💧 :droplet:
👂 :ear:	👀 :eyes:	👃 :nose:
👅 :tongue:	💌 :love_letter:	👤 :bust_in_silhouette:
👥 :busts_in_silhouette:	💬 :speech_balloon:	💭 :thought_balloon:
Nature
☀️ :sunny:	☔️ :umbrella:	☁️ :cloud:
❄️ :snowflake:	⛄️ :snowman:	⚡️ :zap:
🌀 :cyclone:	🌁 :foggy:	🌊 :ocean:
🐱 :cat:	🐶 :dog:	🐭 :mouse:
🐹 :hamster:	🐰 :rabbit:	🐺 :wolf:
🐸 :frog:	🐯 :tiger:	🐨 :koala:
🐻 :bear:	🐷 :pig:	🐽 :pig_nose:
🐮 :cow:	🐗 :boar:	🐵 :monkey_face:
🐒 :monkey:	🐴 :horse:	🐎 :racehorse:
🐫 :camel:	🐑 :sheep:	🐘 :elephant:
🐼 :panda_face:	🐍 :snake:	🐦 :bird:
🐤 :baby_chick:	🐥 :hatched_chick:	🐣 :hatching_chick:
🐔 :chicken:	🐧 :penguin:	🐢 :turtle:
🐛 :bug:	🐝 :honeybee:	🐜 :ant:
🐞 :beetle:	🐌 :snail:	🐙 :octopus:
🐠 :tropical_fish:	🐟 :fish:	🐳 :whale:
🐋 :whale2:	🐬 :dolphin:	🐄 :cow2:
🐏 :ram:	🐀 :rat:	🐃 :water_buffalo:
🐅 :tiger2:	🐇 :rabbit2:	🐉 :dragon:
🐐 :goat:	🐓 :rooster:	🐕 :dog2:
🐖 :pig2:	🐁 :mouse2:	🐂 :ox:
🐲 :dragon_face:	🐡 :blowfish:	🐊 :crocodile:
🐪 :dromedary_camel:	🐆 :leopard:	🐈 :cat2:
🐩 :poodle:	🐾 :paw_prints:	💐 :bouquet:
🌸 :cherry_blossom:	🌷 :tulip:	🍀 :four_leaf_clover:
🌹 :rose:	🌻 :sunflower:	🌺 :hibiscus:
🍁 :maple_leaf:	🍃 :leaves:	🍂 :fallen_leaf:
🌿 :herb:	🍄 :mushroom:	🌵 :cactus:
🌴 :palm_tree:	🌲 :evergreen_tree:	🌳 :deciduous_tree:
🌰 :chestnut:	🌱 :seedling:	🌼 :blossom:
🌾 :ear_of_rice:	🐚 :shell:	🌐 :globe_with_meridians:
🌞 :sun_with_face:	🌝 :full_moon_with_face:	🌚 :new_moon_with_face:
🌑 :new_moon:	🌒 :waxing_crescent_moon:	🌓 :first_quarter_moon:
🌔 :waxing_gibbous_moon:	🌕 :full_moon:	🌖 :waning_gibbous_moon:
🌗 :last_quarter_moon:	🌘 :waning_crescent_moon:	🌜 :last_quarter_moon_with_face:
🌛 :first_quarter_moon_with_face:	🌔 :moon:	🌍 :earth_africa:
🌎 :earth_americas:	🌏 :earth_asia:	🌋 :volcano:
🌌 :milky_way:	⛅️ :partly_sunny:	 
Object
🎍 :bamboo:	💝 :gift_heart:	🎎 :dolls:
🎒 :school_satchel:	🎓 :mortar_board:	🎏 :flags:
🎆 :fireworks:	🎇 :sparkler:	🎐 :wind_chime:
🎑 :rice_scene:	🎃 :jack_o_lantern:	👻 :ghost:
🎅 :santa:	🎄 :christmas_tree:	🎁 :gift:
🔔 :bell:	🔕 :no_bell:	🎋 :tanabata_tree:
🎉 :tada:	🎊 :confetti_ball:	🎈 :balloon:
🔮 :crystal_ball:	💿 :cd:	📀 :dvd:
💾 :floppy_disk:	📷 :camera:	📹 :video_camera:
🎥 :movie_camera:	💻 :computer:	📺 :tv:
📱 :iphone:	☎️ :phone:	☎️ :telephone:
📞 :telephone_receiver:	📟 :pager:	📠 :fax:
💽 :minidisc:	📼 :vhs:	🔉 :sound:
🔈 :speaker:	🔇 :mute:	📢 :loudspeaker:
📣 :mega:	⌛️ :hourglass:	⏳ :hourglass_flowing_sand:
⏰ :alarm_clock:	⌚️ :watch:	📻 :radio:
📡 :satellite:	➿ :loop:	🔍 :mag:
🔎 :mag_right:	🔓 :unlock:	🔒 :lock:
🔏 :lock_with_ink_pen:	🔐 :closed_lock_with_key:	🔑 :key:
💡 :bulb:	🔦 :flashlight:	🔆 :high_brightness:
🔅 :low_brightness:	🔌 :electric_plug:	🔋 :battery:
📲 :calling:	✉️ :email:	📫 :mailbox:
📮 :postbox:	🛀 :bath:	🛁 :bathtub:
🚿 :shower:	🚽 :toilet:	🔧 :wrench:
🔩 :nut_and_bolt:	🔨 :hammer:	💺 :seat:
💰 :moneybag:	💴 :yen:	💵 :dollar:
💷 :pound:	💶 :euro:	💳 :credit_card:
💸 :money_with_wings:	📧 :e-mail:	📥 :inbox_tray:
📤 :outbox_tray:	✉️ :envelope:	📨 :incoming_envelope:
📯 :postal_horn:	📪 :mailbox_closed:	📬 :mailbox_with_mail:
📭 :mailbox_with_no_mail:	🚪 :door:	🚬 :smoking:
💣 :bomb:	🔫 :gun:	🔪 :hocho:
💊 :pill:	💉 :syringe:	📄 :page_facing_up:
📃 :page_with_curl:	📑 :bookmark_tabs:	📊 :bar_chart:
📈 :chart_with_upwards_trend:	📉 :chart_with_downwards_trend:	📜 :scroll:
📋 :clipboard:	📆 :calendar:	📅 :date:
📇 :card_index:	📁 :file_folder:	📂 :open_file_folder:
✂️ :scissors:	📌 :pushpin:	📎 :paperclip:
✒️ :black_nib:	✏️ :pencil2:	📏 :straight_ruler:
📐 :triangular_ruler:	📕 :closed_book:	📗 :green_book:
📘 :blue_book:	📙 :orange_book:	📓 :notebook:
📔 :notebook_with_decorative_cover:	📒 :ledger:	📚 :books:
🔖 :bookmark:	📛 :name_badge:	🔬 :microscope:
🔭 :telescope:	📰 :newspaper:	🏈 :football:
🏀 :basketball:	⚽️ :soccer:	⚾️ :baseball:
🎾 :tennis:	🎱 :8ball:	🏉 :rugby_football:
🎳 :bowling:	⛳️ :golf:	🚵 :mountain_bicyclist:
🚴 :bicyclist:	🏇 :horse_racing:	🏂 :snowboarder:
🏊 :swimmer:	🏄 :surfer:	🎿 :ski:
♠️ :spades:	♥️ :hearts:	♣️ :clubs:
♦️ :diamonds:	💎 :gem:	💍 :ring:
🏆 :trophy:	🎼 :musical_score:	🎹 :musical_keyboard:
🎻 :violin:	👾 :space_invader:	🎮 :video_game:
🃏 :black_joker:	🎴 :flower_playing_cards:	🎲 :game_die:
🎯 :dart:	🀄️ :mahjong:	🎬 :clapper:
📝 :memo:	📝 :pencil:	📖 :book:
🎨 :art:	🎤 :microphone:	🎧 :headphones:
🎺 :trumpet:	🎷 :saxophone:	🎸 :guitar:
👞 :shoe:	👡 :sandal:	👠 :high_heel:
💄 :lipstick:	👢 :boot:	👕 :shirt:
👕 :tshirt:	👔 :necktie:	👚 :womans_clothes:
👗 :dress:	🎽 :running_shirt_with_sash:	👖 :jeans:
👘 :kimono:	👙 :bikini:	🎀 :ribbon:
🎩 :tophat:	👑 :crown:	👒 :womans_hat:
👞 :mans_shoe:	🌂 :closed_umbrella:	💼 :briefcase:
👜 :handbag:	👝 :pouch:	👛 :purse:
👓 :eyeglasses:	🎣 :fishing_pole_and_fish:	☕️ :coffee:
🍵 :tea:	🍶 :sake:	🍼 :baby_bottle:
🍺 :beer:	🍻 :beers:	🍸 :cocktail:
🍹 :tropical_drink:	🍷 :wine_glass:	🍴 :fork_and_knife:
🍕 :pizza:	🍔 :hamburger:	🍟 :fries:
🍗 :poultry_leg:	🍖 :meat_on_bone:	🍝 :spaghetti:
🍛 :curry:	🍤 :fried_shrimp:	🍱 :bento:
🍣 :sushi:	🍥 :fish_cake:	🍙 :rice_ball:
🍘 :rice_cracker:	🍚 :rice:	🍜 :ramen:
🍲 :stew:	🍢 :oden:	🍡 :dango:
🥚 :egg:	🍞 :bread:	🍩 :doughnut:
🍮 :custard:	🍦 :icecream:	🍨 :ice_cream:
🍧 :shaved_ice:	🎂 :birthday:	🍰 :cake:
🍪 :cookie:	🍫 :chocolate_bar:	🍬 :candy:
🍭 :lollipop:	🍯 :honey_pot:	🍎 :apple:
🍏 :green_apple:	🍊 :tangerine:	🍋 :lemon:
🍒 :cherries:	🍇 :grapes:	🍉 :watermelon:
🍓 :strawberry:	🍑 :peach:	🍈 :melon:
🍌 :banana:	🍐 :pear:	🍍 :pineapple:
🍠 :sweet_potato:	🍆 :eggplant:	🍅 :tomato:
🌽 :corn:	 	 
```

#### 2.Places

```
🏠 :house:	🏡 :house_with_garden:	🏫 :school:
🏢 :office:	🏣 :post_office:	🏥 :hospital:
🏦 :bank:	🏪 :convenience_store:	🏩 :love_hotel:
🏨 :hotel:	💒 :wedding:	⛪️ :church:
🏬 :department_store:	🏤 :european_post_office:	🌇 :city_sunrise:
🌆 :city_sunset:	🏯 :japanese_castle:	🏰 :european_castle:
⛺️ :tent:	🏭 :factory:	🗼 :tokyo_tower:
🗾 :japan:	🗻 :mount_fuji:	🌄 :sunrise_over_mountains:
🌅 :sunrise:	🌠 :stars:	🗽 :statue_of_liberty:
🌉 :bridge_at_night:	🎠 :carousel_horse:	🌈 :rainbow:
🎡 :ferris_wheel:	⛲️ :fountain:	🎢 :roller_coaster:
🚢 :ship:	🚤 :speedboat:	⛵️ :boat:
⛵️ :sailboat:	🚣 :rowboat:	⚓️ :anchor:
🚀 :rocket:	✈️ :airplane:	🚁 :helicopter:
🚂 :steam_locomotive:	🚊 :tram:	🚞 :mountain_railway:
🚲 :bike:	🚡 :aerial_tramway:	🚟 :suspension_railway:
🚠 :mountain_cableway:	🚜 :tractor:	🚙 :blue_car:
🚘 :oncoming_automobile:	🚗 :car:	🚗 :red_car:
🚕 :taxi:	🚖 :oncoming_taxi:	🚛 :articulated_lorry:
🚌 :bus:	🚍 :oncoming_bus:	🚨 :rotating_light:
🚓 :police_car:	🚔 :oncoming_police_car:	🚒 :fire_engine:
🚑 :ambulance:	🚐 :minibus:	🚚 :truck:
🚋 :train:	🚉 :station:	🚆 :train2:
🚅 :bullettrain_front:	🚄 :bullettrain_side:	🚈 :light_rail:
🚝 :monorail:	🚃 :railway_car:	🚎 :trolleybus:
🎫 :ticket:	⛽️ :fuelpump:	🚦 :vertical_traffic_light:
🚥 :traffic_light:	⚠️ :warning:	🚧 :construction:
🔰 :beginner:	🏧 :atm:	🎰 :slot_machine:
🚏 :busstop:	💈 :barber:	♨️ :hotsprings:
🏁 :checkered_flag:	🎌 :crossed_flags:	🏮 :izakaya_lantern:
🗿 :moyai:	🎪 :circus_tent:	🎭 :performing_arts:
📍 :round_pushpin:	🚩 :triangular_flag_on_post:	🇯🇵 :jp:
🇰🇷 :kr:	🇨🇳 :cn:	🇺🇸 :us:
🇫🇷 :fr:	🇪🇸 :es:	🇮🇹 :it:
🇷🇺 :ru:	🇬🇧 :gb:	🇬🇧 :uk:
🇩🇪 :de:	 	 
```

#### 3.Symbols

```
1️⃣ :one:	2️⃣ :two:	3️⃣ :three:
4️⃣ :four:	5️⃣ :five:	6️⃣ :six:
7️⃣ :seven:	8️⃣ :eight:	9️⃣ :nine:
🔟 :keycap_ten:	🔢 :1234:	0️⃣ :zero:
#️⃣ :hash:	🔣 :symbols:	◀️ :arrow_backward:
⬇️ :arrow_down:	▶️ :arrow_forward:	⬅️ :arrow_left:
🔠 :capital_abcd:	🔡 :abcd:	🔤 :abc:
↙️ :arrow_lower_left:	↘️ :arrow_lower_right:	➡️ :arrow_right:
⬆️ :arrow_up:	↖️ :arrow_upper_left:	↗️ :arrow_upper_right:
⏬ :arrow_double_down:	⏫ :arrow_double_up:	🔽 :arrow_down_small:
⤵️ :arrow_heading_down:	⤴️ :arrow_heading_up:	↩️:leftwards_arrow_with_hook:
↪️ :arrow_right_hook:	↔️ :left_right_arrow:	↕️ :arrow_up_down:
🔼 :arrow_up_small:	🔃 :arrows_clockwise:	🔄 :arrows_counterclockwise:
⏪ :rewind:	⏩ :fast_forward:	ℹ️ :information_source:
🆗 :ok:	🔀 :twisted_rightwards_arrows:	🔁 :repeat:
🔂 :repeat_one:	🆕 :new:	🔝 :top:
🆙 :up:	🆒 :cool:	🆓 :free:
🆖 :ng:	🎦 :cinema:	🈁 :koko:
📶 :signal_strength:	🈹 :u5272:	🈴 :u5408:
🈺 :u55b6:	🈯️ :u6307:	🈷️ :u6708:
🈶 :u6709:	🈵 :u6e80:	🈚️ :u7121:
🈸 :u7533:	🈳 :u7a7a:	🈲 :u7981:
🈂️ :sa:	🚻 :restroom:	🚹 :mens:
🚺 :womens:	🚼 :baby_symbol:	🚭 :no_smoking:
🅿️ :parking:	♿️ :wheelchair:	🚇 :metro:
🛄 :baggage_claim:	🉑 :accept:	🚾 :wc:
🚰 :potable_water:	🚮 :put_litter_in_its_place:	㊙️ :secret:
㊗️ :congratulations:	Ⓜ️ :m:	🛂 :passport_control:
🛅 :left_luggage:	🛃 :customs:	🉐 :ideograph_advantage:
🆑 :cl:	🆘 :sos:	🆔 :id:
🚫 :no_entry_sign:	🔞 :underage:	📵 :no_mobile_phones:
🚯 :do_not_litter:	🚱 :non-potable_water:	🚳 :no_bicycles:
🚷 :no_pedestrians:	🚸 :children_crossing:	⛔️ :no_entry:
✳️ :eight_spoked_asterisk:	✴️ :eight_pointed_black_star:	💟 :heart_decoration:
🆚 :vs:	📳 :vibration_mode:	📴 :mobile_phone_off:
💹 :chart:	💱 :currency_exchange:	♈️ :aries:
♉️ :taurus:	♊️ :gemini:	♋️ :cancer:
♌️ :leo:	♍️ :virgo:	♎️ :libra:
♏️ :scorpius:	♐️ :sagittarius:	♑️ :capricorn:
♒️ :aquarius:	♓️ :pisces:	⛎ :ophiuchus:
🔯 :six_pointed_star:	❎:negative_squared_cross_mark:	🅰️ :a:
🅱️ :b:	🆎 :ab:	🅾️ :o2:
💠:diamond_shape_with_a_dot_inside:	♻️ :recycle:	🔚 :end:
🔛 :on:	🔜 :soon:	🕐 :clock1:
🕜 :clock130:	🕙 :clock10:	🕥 :clock1030:
🕚 :clock11:	🕦 :clock1130:	🕛 :clock12:
🕧 :clock1230:	🕑 :clock2:	🕝 :clock230:
🕒 :clock3:	🕞 :clock330:	🕓 :clock4:
🕟 :clock430:	🕔 :clock5:	🕠 :clock530:
🕕 :clock6:	🕡 :clock630:	🕖 :clock7:
🕢 :clock730:	🕗 :clock8:	🕣 :clock830:
🕘 :clock9:	🕤 :clock930:	💲 :heavy_dollar_sign:
©️ :copyright:	®️ :registered:	™️ :tm:
❌ :x:	❗️ :heavy_exclamation_mark:	‼️ :bangbang:
⁉️ :interrobang:	⭕️ :o:	✖️ :heavy_multiplication_x:
➕ :heavy_plus_sign:	➖ :heavy_minus_sign:	➗ :heavy_division_sign:
💮 :white_flower:	💯 :100:	✔️ :heavy_check_mark:
☑️ :ballot_box_with_check:	🔘 :radio_button:	🔗 :link:
➰ :curly_loop:	〰️ :wavy_dash:	〽️ :part_alternation_mark:
🔱 :trident:	:black_square: :black_square:	:white_square: :white_square:
✅ :white_check_mark:	🔲 :black_square_button:	🔳 :white_square_button:
⚫️ :black_circle:	⚪️ :white_circle:	🔴 :red_circle:
🔵 :large_blue_circle:	🔷 :large_blue_diamond:	🔶 :large_orange_diamond:
🔹 :small_blue_diamond:	🔸 :small_orange_diamond:	🔺 :small_red_triangle:
🔻 :small_red_triangle_down:	 	 
```





### 6、Typora常见配置

#### 1.本地编辑md文件一般配置方法(已解决)

默认情况，Typora软件会把粘贴进去的图片copy到pc c盘的一个目录下面；

因此，我们会推荐采用使用相对路径来存放当前md文件里的图片；

```
./${filename}_md_pictures  #这个代表如何md文件里面有插入图片的话，typora会在该文件的当前目录下生成一个同名目录来专门存放图片数据的
```

![image-20210130233726210](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130233726210.png)
![image-20210130233742530](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130233742530.png)

#### 2.配置自动保存功能(已解决)

![image-20210130233848464](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210130233848464.png)



#### 3.更改字体、大小、颜色、背景色(已解决)

**（1）更改字体、大小、颜色**

<font face="黑体">我是黑体字</font> <font face="微软雅黑">我是微软雅黑</font> <font face="STCAIYUN">我是华文彩云</font> <font color=red>我是红色</font> <font color=#008000>我是绿色</font> <font color=Blue>我是蓝色</font> <font size=5>我是尺寸</font> <font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>

```bash
<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>

<font color=red>我是红色</font>
<font color=#008000>我是绿色</font>
<font color=Blue>我是蓝色</font>

<font size=5>我是尺寸</font>

<font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>
```



**（2）更改背景色**

01、

<table><tr><td bgcolor=red>背景色red</td></tr></table>

```html
<table><tr><td bgcolor=red>背景色red</td></tr></table>
```



02、

<span style='color:yellow;background:red;font-size:14;font-family:字体;'>文字</span>

```bash
<span style='color:yellow;background:red;font-size:文字大小;font-family:字体;'>文字</span>
```

#### 3.侧边栏的大纲视图允许折叠和展开(已解决)

![image-20210131170715734](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210131170715734.png)

![image-20210131170605243](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210131170605243.png)

#### 4.picgo如果配置的是阿里云oss图床的话，那么很轻松可以在typora里一次性上传本地所有图片的；-20211107(已完成)`完美`(已解决)

> 注意：前提是oss里的图片名称不能存在，否则会上传报错的！！！

![image-20211107064000219](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211107064000219.png)

#### 5.TS：typora导出word方法(成功测试)？-2021.4.28(已解决)

![image-20210428122252430](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428122252430.png)

![image-20210428122346063](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428122346063.png)

![image-20210428122415545](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428122415545.png)

![image-20210428122841754](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428122841754.png)

![image-20210428122902538](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428122902538.png)

安装完pandoc后，重启typora软件，再次导出即可：

![image-20210428123050722](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428123050722.png)

![image-20210428123057647](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428123057647.png)

![image-20210428123121028](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210428123121028.png)

#### 6.TS：我淦-typora的代码出现了格式问题-2021.11.30(已解决)

##### 1、问题现象

我淦，typora的代码快里的代码出现了换行乱序问题。。。好无语。。。

![image-20211130141916852](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130141916852.png)



奇怪的是：一篇文章里，有的代码块里的代码乱序了，有的没乱序，这个就很奇怪了。。。

![image-20211130142038691](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130142038691.png)

##### 2、排查过程

:warning:

重新在一个新winodws环境安装typora后，其默认的换行是`CRLF`，缩进是`2`。

自己之前重新修改过typora的设置，修改结果为：换行是`LF`，缩进是`4`。

个人判断就是这个原因导致的结果。。。



- typora安装后默认的换行符及缩进：

![image-20211130142619050](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130142619050.png)



- 个人typora故障时自己的环境

自己现在的版本是正式版本：1.0.2，之前老的版本也偶尔看到了这个问题。。

![image-20211130142808462](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130142808462.png)



##### 3、解决办法

1. 将自己现在的2个笔记本的typora软件的`换行符和缩进`全部改成默认属性

   ![image-20211130143031963](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130143031963.png)

2. 下次再进行大量赋值粘贴后，必须查看代码是否存在`乱序问题`；

##### 4、验证效果

修改为原来安装属性后，我们来确认下是否会对最近编写的文档里的代码是否有影响？

这里随机查看下2个文档：

![image-20211130143624310](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130143624310.png)

![image-20211130143709665](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211130143709665.png)



随机查看了2个文档，格式都是没任何问题的。

这个遗留问题后续再观察现象即可。
