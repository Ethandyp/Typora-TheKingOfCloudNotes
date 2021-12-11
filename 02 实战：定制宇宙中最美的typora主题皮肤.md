## 实战：定制宇宙中最美的typora主题皮肤-2021.12.07

![image-20211207110726837](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207110726837.png)

## 文档更新时间log

- 2021年12月11日09:32:37

  更新内容：修改typora编辑界面边框阴影颜色为粉色，应该会好看点吧哈哈😂，主题文件为`lovexyy-2021.12.11.css`。

## 1、最新版typora主题版本css文件位置

(1)我们先来看下这个`lovexyy-2021.12.11.css`主题md文件效果

![image-20211211093811686](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211211093811686.png)

![image-20211211093958839](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211211093958839.png)



(2)最新版css主题文件位置

`2021.12.03-typora相关软件`

链接：https://pan.baidu.com/s/19Calca7xkjjYbOwX0YGBBw 
提取码：wqb8 
--来自百度网盘超级会员V6的分享

记得要安装`FiraCode、OperatorMono`字体哦。

![image-20211211094314188](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211211094314188.png)

![image-20211211094341931](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211211094341931.png)



(3)使用方法：将这个主题文件放到typora的主体路径下，重启typora即可

`文件-偏好设置-外观-打开主题文件夹`

关于云笔记的搭建及使用方法可参考我的开源项目：`https://github.com/OnlyOnexl/Typora-TheKingOfCloudNotes`

![image-20211204151903738](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211204151903738.png)

## 2、typora主题定制细节

![](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125160712620.png)

### :pushpin:定义的是界面颜色、文字颜色(配置护眼绿)：`root字段`(已完成)

```bash
#说明
root里定义的是界面颜色、文字颜色等。

text-color：文字颜色
bg-color：背景颜色
code-block-bg-color：代码块颜色
side-bar-bg-color：文件夹、大纲处的颜色
window-border：窗口边界颜色
```



- 案例1

  ```css
  :root {
      --text-color: #666;
      --bg-color: #fff;
      --code-block-bg-color: #4d4d4d;
      --side-bar-bg-color: #fdf6f5;
      --window-border: 1px solid #555;
      
      --active-file-bg-color: #fff;
      --active-file-text-color: #666;
      --item-hover-text-color: #666;
      --control-text-color: #777;
      }
  ```

  ![image-20211126144232123](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144232123.png)

  效果图如下：

  ![image-20211126144325605](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144325605.png)

- 案例2

  ```css
  :root {
      --side-bar-bg-color: #c7e6c8;
      --control-text-color: #777;
  	#background-color: #c7edcc;
  	background: url('./bg_image/v-34.png')  repeat
  }
  ```

  ![image-20211126144415434](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144415434.png)

  ![image-20211126144450354](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144450354.png)

  是600*600大小的图片：

  ![](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144522824.png)

  效果如下：

  ![image-20211126144621365](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126144621365.png)

  完美。

### :pushpin:正文字体大小及字体类型(配置好看的字体)配置：`body字段`(已完成)

- 案例

  ```cs
  html {
      font-size: 18px;
  }
  
  body {
      font-family: "华康手札体W5P",'Microsoft YaHei',"SimSun","Clear Sans","Helvetica Neue",Helvetica,Arial,sans-serif;
      color: rgb(51, 51, 51);
      line-height: 1.6;
  }
  ```

  ![image-20211126150309858](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126150309858.png)

- 效果

  ![image-20211126150339159](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126150339159.png)



### :pushpin:定制typora主题css文件

使用typora的时候，想要自定义一些颜色、字体，或者修改一些设置，这个时候需要修改或者自己编写css文件。

打开文件 - 偏好设置 - 外观 - 打开主题文件夹，选择你自己的主题名.css（默认是 Github.css），在最后插入 CSS 代码，保存退出，再次打开typora文件即可；

![image-20210131103924364](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210131103924364-16281470339701.png)

![image-20210719101713575](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210719101713575.png)

![image-20210719101737328](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210719101737328.png)

### :pushpin:正文字体大小及字体类型配置：`font`(已完成)

1. 配置方法

   ![image-20211121082733098](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121082733098.png)

   ```css
   /* 正文字体大小及字体类型配置 */
   html {
       font-size: 16px;
   }
   body {
       font-family: "华康手札体W5P", "Open Sans","Clear Sans","Helvetica Neue",Helvetica,Arial,sans-serif;
       /*color: rgb(51, 51, 51);*/
       background-color: mintcream; /*正文背景颜色*/
       color: rgb(51, 51, 51); /*正文字体颜色*/
       line-height: 1.6;
   }
   ```

2. 配置效果

   1.css主题：

   ![image-20211121082840852](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121082840852.png)

### :pushpin:设置图片默认左对齐：`image`(已完成)

- 默认情况，Typora的图片是居中对齐的。

- 现在有个需求，想让每次哦插入的图片都默认做对齐，该如何实现呢？

- 设置方法

  打开文件 - 偏好设置 - 外观 - 打开主题文件夹，选择你自己的主题名.css（默认是 Github.css），在最后插入 CSS 代码，保存退出，再次打开typora文件即可：

  ![image-20211120220641317](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211120220641317.png)

  ```css
  /*设置图片默认左对齐：在css文件末尾追加即可*/
  p .md-image:only-child{
      width: auto;
      text-align: left;
      }
  ```

- 观察效果

  符合预期效果。

  ![image-20211120220914580](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211120220914580.png)



### :pushpin:引用段落：`quote`(已完成)

- 修改位置

![image-20211120215749938](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211120215749938.png)

```css
blockquote {
    border-left: 4px solid #8080ff; /*侧边小竖条的颜色 */
    padding: 0 15px;
    color: black; /*引用段落字体颜色*/
    background-color: #deb887; /*引用段落背景颜色*/
}
```



- 效果如下

> 引用段落。

![image-20211120215829239](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211120215829239.png)

### :pushpin:修改typora编辑区域左右间距方法：`write`(已完成)

1. 配置方法

   ![image-20211121084649932](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121084649932.png)

   ```cs
   #write{
       max-width: 960px; /*注意这个是控制编辑的宽度的：可以是100%，980px；*/
       margin-top:    30px; /*top*/
       margin-bottom: 30px;
       padding: 100px 60px; /*top to title padding*/
       border-radius: 5px;
       -o-box-shadow: 0 10px 10px #333333;
       -webkit-box-shadow: 0 10px 10px #333333;
       -moz-box-shadow: 0 10px 10px #333333;
       box-shadow: 0px 50px 100px #333333;
   }
   #write > ul:first-child,
   #write > ol:first-child{
       margin-top: 30px;
   }
   ```

2. 验证效果

   ![image-20211121084742015](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121084742015.png)


### :pushpin:模拟mac的三个图标：（已完成）

1.案例

![image-20211126150748053](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126150748053.png)

![image-20211126150813478](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126150813478.png)

```css
/* MAC的三个图标 */
.CodeMirror-wrap .CodeMirror-scroll {
    padding-top: 20px;
}
 
#write .md-fences:before {
    content: "";
    z-index: 4;
    display: block;
    position: absolute;
    top: 7px;
    left: 13px;
    width: 15px;
    height: 15px;
    border-radius: 50%;
    float: left;
    background-color: #fa3534;
}
 
#write .CodeMirror-scroll:before {
    content: "";
    display: block;
    position: absolute;
    top: 0px;
    left: 29px;
    width: 15px;
    height: 15px;
    border-radius: 50%;
    float: left;
    z-index: 999;
    background-color: #ff9900;
}
#write .md-fences::after {
    content: "";
    z-index: 4;
    display: block;
    position: absolute;
    top: 7px;
    left: 53px;
    width: 15px;
    height: 15px;
    border-radius: 50%;
    float: left;
    background-color: #19be6b;
}
```

效果

![image-20211126150844217](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126150844217.png)

### :pushpin:选中文字部分颜色修改：`selection`(已完成)

1.配置方法

![image-20211121085538860](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121085538860.png)

```cs
/* 选中文字部分颜色修改 */
::selection {
    background-color: #d1ff79;
}
```



2.验证效果

![image-20211121085617973](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121085617973.png)

### :pushpin:修改标题颜色：`h1-h6`(已完成)

1.配置方法

![image-20211121085254716](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121085254716.png)

```cs
h1,
h2,
h3,
h4,
h5,
h6 {
    position: relative;
    margin-top: 1rem;
    margin-bottom: 1rem;
    font-weight: bold;
    line-height: 1.4;
    cursor: text;
    color: #4169E1; /*配置h1-h6级标题颜色*/
}
```



2.验证效果

![image-20211121085326262](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211121085326262.png)

### :pushpin:选中文字部分颜色修改:`selection字段`(已完成)

在css文件最后添加

![image-20211126152331960](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126152331960.png)

```bash
::selection {
    background-color: #d1ff79;
}
```



效果如下：

![image-20211126152407900](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126152407900.png)

### :pushpin:部分文字标红：`mark字段`(已完成)

1、配置方法

![image-20211126152658804](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126152658804.png)

![image-20211126152923142](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126152923142.png)

```css
/*==背景高亮==,mark是符号==xxx==的效果*/
mark {
    background: rgb(0, 255, 85);
    color: #f22f27;
    font-weight: bold;
    border-bottom: 0px solid #ffffff;
    padding: 0.0px;
    margin: 0 0px;
  }
```



2、效果如下：

==我爱中国==

![image-20211126153000495](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126153000495.png)

### :pushpin:链接：(已配置)

1、配置方法

![image-20211126153149055](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126153149055.png)

```bash
/* 链接 */
#write a {
    color: #f22f27;
    text-decoration: none;
    border-bottom: 1px solid #f22f27;
} 

/* 链接内容为空时直接啥也不显示，比如锚点的地方 */
#write a:empty {
  font-size: 0;
  border: none;
}
```



2、效果 如下：

https://www.baudu.com

### :pushpin:修改代码背景颜色为sublime text3的背景色：(已完成)

1、配置方法

注意：sublimet text3背景颜色的颜色代码为

```bash
background: #232323; 这个颜色为sublime text3的颜色；
```

![image-20210623141801208](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210623141801208.png)

![image-20211126163919759](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126163919759.png)

```css
/*深色背景*/
 
#write .md-fences:not([mermaid-type])  {
    padding-top: 7px;
    border-radius: 10px;
    background-color: #232323;
    color: #eeeeee;
}
```



2、查看效果

![image-20211126163958460](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126163958460.png)

### :question:markdown nice这种好看的主体如何定制到typora里面来？

![image-20211126153705296](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126153705296.png)

![image-20211007204338324](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211007204338324.png)

![image-20211126153731499](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211126153731499.png)

### 📍 实战：修改Typora默认的字体为好看秀美的中文字体华康手札体并配置一些高级定制功能(成功测试-博客输出)-2021.04.04

#### 本次测试环境

```bash
winodws10操作系统
typora软件：0.0.98（相近版本一般都可以进行验证操作）
```

#### 软件位置

![image-20210805151709273](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805151709273.png)

#### 1.请客官先体验下最终效果图

大家可先瞅一瞅最终修改后的效果图如何，再根据自己需求是否决定要更改为如下的字体**"华康手札体W5P"**：

![image-20210404063826013](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404063826013.png)

个人觉得"华康手札体W5P"字体还是比较秀美的，哈哈。

#### 2.需求产生

- typora默认的那个"Open Sans"字体，自己感觉不是很美观啊，虽然可以接受，但总觉得缺了些什么。。


![image-20210404064034226](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404064034226.png)

![image-20210404064059704](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404064059704.png)



- 上次修改的Typora的**微软雅黑**这个字体，用了一段时间发现真的也很丑啊。。。。。（呃呃，默认的"Open Scan"字体怎么感觉和微软雅黑看起来没啥区别啊。。。。）


![image-20210404064216188](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404064216188.png)

![image-20210403231230989](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210403231230989.png)



- 因此，现在想要更换一款比较好看的字体：于是，上网搜了下，找了许久，发现一个博主写的"华康手札体W5P"这个字体不错，很秀美，因此下面将实现这种需求。
  本次参考博客链接如下：https://blog.csdn.net/a2352159950/article/details/108153531

![image-20210403231356070](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210403231356070.png)

因此接下来参考这个博主的博客进行自定义自己的typora字体。

#### 3.更改方法

#### 3.1 下载并安装"华康手札体W5P"字体

hannotate是什么字体？hannotate sc regular字体又叫手札体 简 常规标准体，这款字体字形清秀工整，线条流畅洒脱，笔形富于变化。

你可以百度"华康手札体W5P字体进行下载或者从如下百度云链接进行获取：

1.http://www.downcc.com/font/341067.html （但是这个虽然叫做绿色下载网站，但是下载后附带一大波软件，无语了。。。。。）
2.百度云链接：

链接：https://pan.baidu.com/s/125Hh-tqWOy1Ht-GvD_P2MQ 
提取码：z6ka 
复制这段内容后打开百度网盘手机App，操作更方便哦--来自百度网盘超级会员V6的分享

将压缩包解压后，直接把`华康手札体w5.ttf`文件复制到windows下的`C:\WINDOWS\Fonts`目录下即可。

![image-20210404065421073](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404065421073.png)

#### 3.2 修改Typora默认的字体为好看秀美的中文字体"华康手札体"

我的Typora使用的是github这个主题(**不同的主题只需要在相应的.css文件中进行同样的修改即可**)，我将以它为例（这里用mac界面展示，win也是一样的）

1.首先打开typora的偏好设置，在外观中找到主题文件夹，打开这个文件夹

![image-20210404065633823](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404065633823.png)

2.打开github.css文件

![image-20210404065706196](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404065706196.png)

3.这里是修改字体的，找到下面的代码位置，**将"华康手札体W5P"添加到下面的位置，一定要放在最前面**
(注意，如果改了字体却并未生效，说明你电脑里面没有"华康手札体W5P"这个字体，可以百度搜一下手札体下载，下载解压安装，重启typora即可生效）

+++

**这里需要注意**：网上其实也有一些关于Typora换字体的文章，但是大多都有一个问题——**中文字体无法正常显示问题**。下面将详细说明如何解决这个问题；（一般是给出2中方法，推荐后面那一种）

Typora的各种属性都是在主题文件中定义的，实际上Typora就是一个带编辑功能的浏览器，其主题文件就是一个个.css文件；
知道了这一点，学过前端的朋友可能就懂了，虽然我没学过前端。。只是略懂一些网页的渲染原理;
在这个文件夹下面有几个子文件夹和几个.css文件，实际上这些css就是主题，文件名就是主题名称;

然后在下面几行有一个body里面定义了一个font-family，这个就是字体的定义了:

![image-20210404070727160](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404070727160.png)

在 font-family 后面加一个自己的字体试试？比如 “宋体” 像这样。

注意双引号和逗号 ！！

![image-20210404070908139](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404070908139.png)

重启Typora并选择github主题，你会发现字体并没有变化，这是因为typora现在并不认识中文。**别的教程说的是使用字体的英文名称**，比如“微软雅黑”是“Microsoft Yahei”
——这不失为一种解决方案，但是我个人认为，微软雅黑也并不好看。

所以，在花了一个下午，研究了其他的主题换字体的方式后，我发现——其他的主题也全™是用的英文。。。于是又试了很多方案，在试的过程中无意发现浏览器里面的源码里面可以有中文注释，浏览器是怎么认识中文的呢？
百度一下发现**css文档前面声明字符集，浏览器就可以识别中文了**，像这样

把这个github.css文件用VScode软件打开：

在VScode底端可以看到文档的字符集是GB2312，**那么就在github.css首行加上**：

```bash
@charset "gb2312"；
```

有可能我在编辑过程中不小心修改了，你的可能和我不一样，最好自己确认一下，如果你的是utf-8,那就加上:

```bash
@charset "UTF-8"；
```

我本次这个是utf-8：

```bash
@charset "UTF-8"；
```

![image-20210404072028674](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404072028674.png)

![image-20210404072447176](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404072447176.png)

再重启Typora看看？感染果然变成了宋体

![image-20210404072134051](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404072134051.png)

以此类推，只要你电脑里面有的字体，就都可以用了。

下面是一些小的注意事项，建议看完。==（如何刚改代码区域字体及背景色？）==
上面的操作修改完，只是body的字体，也就是普通编辑区的字体变成了 “宋体” ，但是还有一些区域还是原来的，比如：

![image-20210404080957672](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404080957672.png)

这个代码块的字体肯定不是我们设置的宋体，那么要怎么改呢？（虽然这个字体挺好看的，貌似MAC里面用的就是这种字体）
继续研究了一段时间发现，**代码的字体是其他的地方限制的**，在github.css的任意地方加上这一段，重启typora：

```bash
.CodeMirror div.CodeMirror-code {
    background-color: rgb(195, 195, 195);
    font-family: "宋体";
}
```

其中background-color是设置代码块的背景颜色，效果就是这样：

![image-20210404081150422](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404081150422.png)

**这里只是作为演示，代码块这一文字我这里就保持默认了，感觉默认挺好看的**。

代码块颜色就比较突出了，怎么样？是不是很棒？

+++

按照上面方法，把字体换成本次要使用的：

![image-20210404072608789](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404072608789.png)

重启typora查看效果：

![image-20210404072642393](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404072642393.png)

已经更换成功，完美！！！

#### 3.3 定制Typora高级功能

- **设置标题颜色：**

找到下图的代码文位置，添加红色框框显示的代码，**这里修改的是绿色的标题，你自己也可以设置其他颜色**，可以在网上找一下rgb颜色表，找一个自己喜欢的颜色作为标题颜色:

```bash
color: rgb(26, 143, 55);
```

![image-20210404081622588](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404081622588.png)

![image-20210404081730983](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404081730983.png)



- **部分文字标红**:

先在偏好设置中选中下面这个高亮(建议拓展语法全勾上）

![image-20210404081839168](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404081839168.png)

然后在github.css文件最后一行加入如下代码，用的时候用左右==包围文字就可以标红了，举例：`==要标红的文字==`

```bash
/*==背景高亮==*/
mark {
    background: #ffffff;
    color: #db3f1e;
    font-weight: bold;
    border-bottom: 0px solid #ffffff;
    padding: 0.0px;
    margin: 0 0px;
  }
```

![image-20210404082012589](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404082012589.png)

![image-20210404082040552](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404082040552.png)



- 选中文字部分颜色修改

当选中一段文字之后，颜色编程如下的草绿色

![image-20210404082129997](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404082129997.png)

在github.css中最后一行加上如下代码就可以实现了:

```bash
::selection {
    background-color: #d1ff79;
}
```

![image-20210404082156464](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210404082156464.png)

好了，本次改善typora到此结束了，哈哈。

欢迎点赞

#### 4.总结

typora是一款非常好用的编辑器，可以用坚果云+typora进行自己的笔记同步备份，虽然网页端无法预览图片，但整体使用下来个人感觉还是很不错的。



多谢下面2位博主的文章，本次借鉴了他们的博客，这里表示非常感谢博主的无私分享。



参考文章：

原文链接：https://blog.csdn.net/qq_40522908/article/details/104218707

原文链接: https://blog.csdn.net/a2352159950/article/details/108153531

![image-20210805151416118](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805151416118.png)

### 📍 实战：一定不能错过的 Typora 增强插件 VLOOK-2021.11.26

#### 实战：一定不能错过的 Typora 增强插件 VLOOK-2021.11.26

#### 软件位置

![image-20210806100400558](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210806100400558.png)

#### 1、什么是VLOOK？

![image-20210805152444547](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805152444547.png)

#### 1.让Markdown的自动化排版和交互性上了N个台阶

![image-20210805153321754](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153321754.png)

#### 2.内置多套原创文档主题、字体主题，一键切换，支持私人定制

![image-20210805153404448](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153404448.png)

#### 3.表格排版+:单元格合并、列格式、表格行分组、自动编号…

![image-20210805153437129](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153437129.png)

#### 4.零成本的图片自动排版～题注、高分屏、反色、替换、版式、…

![image-20210805153519811](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153519811.png)

#### 5.火力全开的演示辅助～聚光灯、激光笔、注音…

![image-20210805153542380](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153542380.png)

#### 6.OMG!可以按:大纲、逐章、段落、插图，多维度浏览文档内容

![image-20210805153610688](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153610688.png)

#### 7.完美适配Dark模式，Markdown变得更Cool了

![image-20210805153648469](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805153648469.png)

#### 8.音/视频、标签、引用折叠、高清插图、…30+特性开箱即用

![image-20210805160538503](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805160538503.png)

#### 2、下载与配置

#### Step	1•下载与配置

a. 从 VLOOK™ 在 GitHub(https://github.com/MadMaxChow/VLOOK/releases) 或 Gitee(https://gitee.com/madmaxchow/VLOOK/releases) 的主页下载最新发布的版本
b. 也可直接在项目主页中下载主题文件(https://github.com/MadMaxChow/VLOOK/tree/master/released/theme)（备用链接
(https://gitee.com/madmaxchow/VLOOK/tree/master/released/theme)）

![image-20210805160815829](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805160815829.png)

![image-20210805160910448](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805160910448.png)

#### Step	2•安装并选择主题

![image-20210805160948258](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805160948258.png)

b. 模板文件在哪？在目录 released 下的文件「**VLOOK-Document-Template.md**」，也可直接在项目主页中下载文档模板

(https://github.com/MadMaxChow/VLOOK/tree/master/released)（备用链接

(https://gitee.com/madmaxchow/VLOOK/tree/master/released)）

#### Step	3•应用插件

![image-20210805161028267](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805161028267.png)

![image-20210805161136822](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210805161136822.png)

项目仓库：https://github.com/MadMaxChow/VLOOK

#### 实际测试效果

==不是很理想，图片不能展示到html出来，很奇怪==。。-20210806

![image-20210806100736859](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210806100736859.png)

### 📍 实战：自定义Typora护眼色主题(博客输出-成功测试)-2021.3.27

#### 1.原文链接

https://blog.csdn.net/u011622109/article/details/78313850?utm_source=blogxgwz3

![image-20210327102528556](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327102528556.png)



#### 2.配置方法

![image-20210327103210156](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327103210156.png)

![image-20210327103250902](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327103250902.png)

![image-20210327103304069](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327103304069.png)

![image-20210327103333486](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327103333486.png)

链接：https://pan.baidu.com/s/1q4vhIOLkhHLYaDl1Va3fFw 
提取码：3qz1 
复制这段内容后打开百度网盘手机App，操作更方便哦--来自百度网盘超级会员V6的分享

![image-20210327103347256](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327103347256.png)

#### 3.总结及改进

上述这种方法，自己已测试且有效果，但因个人爱好不同，有不同的需求，因此后续自己可以自定义样式。



**主要是这个字体问题**：默认主体字体是微软雅黑，但新主体字体是宋体。

![image-20210327165315472](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327165315472.png)

![image-20210327165344811](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327165344811.png)



在本次github默认主体，其字体应该是微软雅黑好像，看起来还是比较美观的：

![image-20210327165315472](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327165315472.png)

![image-20210327171414350](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327171414350.png)

但github_yuxl_bg主体中，默认字体好像是宋体，这个看起来就有些不舒服了：

![image-20210327165344811](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327165344811.png)

![image-20210327171501951](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327171501951.png)



测试办法1：因此，在github_yuxl_bg主体主体中直接使用默认github主体的字体，观测效果：（字体还是没改过来。。）

![image-20210327171640691](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327171640691.png)



测试办法2：再次修改，这次换成微软雅黑的字体：终于有效果了，这次字体全部编程微软雅黑了，这个字体看着确实舒服。

```bash
'Microsoft YaHei'
```

![image-20210327172020501](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327172020501.png)

![image-20210327172200679](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327172200679.png)



因此，关于本次自定义主体`github_yuxl_bg`的优点如下：

```bash
背景色变成了护眼色；
标题变成了蓝色；
分割线变成了虚线；
table增加了样式；
导航大纲有高亮显示；
```

![image-20210327172718674](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327172718674.png)

10.如何结合typora+坚果云实现本地笔记维护 & 结合picGo 阿里云oss来上传md笔记到csdn博客？

（1）默认情况，关闭图片上传功能：

![image-20210327175201915](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327175201915.png)

（2）如果有上传到博客需求时，配置如下：打开上传图片到阿里云oss功能，再一键上传本地所有图片。

![image-20210327175235725](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327175235725.png)

![image-20210327175245088](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327175245088.png)

![image-20210327175326097](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327175326097.png)



#### 4.修改次主题的一级标题为左对齐

这个主体，一级标题是居中对齐的，这个有些怪，应该是可以修改css文件来着的：

![image-20210327224539909](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327224539909.png)

本次主体css文件：

![image-20210327224935433](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327224935433.png)

默认主体css文件：

![image-20210327225012294](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327225012294.png)

修改这里为left后，果然变成了向左对齐了，完美：

![image-20210327225202740](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210327225202740.png)

#### 5.如何给typora换一个优美的字体呢？

#### 6.如何给typora换一个其他的官方主题呢？

https://theme.typora.io/

![image-20210328071050734](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328071050734.png)

```go
下载主题压缩包，将压缩包里边的几个文件解压到Typora的自定义主题目录，包括：
pie.css
pie-dark.css
pie（文件夹）
```

- 主题：pie

![image-20210328071412477](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328071412477.png)

更换后效果如下：

![image-20210328071636846](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328071636846.png)

![image-20210328071701032](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328071701032.png)



- 更换主题solarized（更换后效果）

![image-20210328072229003](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328072229003.png)



#### 7改进：如何使这个图片居左对齐呢？

他提供的这个是居左对齐的。

![image-20210328073746309](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328073746309.png)

请看标题5配置方法：

配置后效果如下：

![image-20210328074223541](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20210328074223541.png)
