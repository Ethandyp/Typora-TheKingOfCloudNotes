## 实战：打造一款最强王者云笔记"typora+坚果云+阿里云oss"-2021.12.07

![image-20211207110635653](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207110635653.png)

:warning:搭建过程若遇到什么问题，可以直接联系我哦哈哈：个人微信二维码：x2675263825 （舍得）， qq：2675263825。

![image-20211002091450217](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/20211106144206.png)

## 实验环境

```bash
win10
typora
picgo
阿里云oss
```

## 实验软件

链接：https://pan.baidu.com/s/19Calca7xkjjYbOwX0YGBBw 
提取码：wqb8 
--来自百度网盘超级会员V6的分享

![image-20211207140806163](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207140806163.png)

## 1.下载坚果云并安装

用于存储我们的笔记文件。

https://www.jianguoyun.com/

同步文件的速度特别快，很丝滑，且文档又有历史版本保留功能；年vip199元，空间40g，每年多购买vip，就会多增加12g；总之很良心，用起来很舒服……

![image-20211203155726062](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211203155726062.png)

## 2.下载typora并安装

用于编辑笔记文件。

[Typora下载](https://www.typora.io/#download)

一款良心md软件，是我用过所有云笔记中最舒服的md软件，没有之一！！！(相信我，用上typora，你会爱上它的:cupid:)

![image-20211125161712909](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211125161712909.png)



:warning: 记得最后配置上我正在使用的主体哦，非常棒的一个自定义typora主题：效果如下

![image-20211203213509137](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211203213509137.png)

![image-20211207104922673](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211207104922673.png)

## 3.配置阿里云oss作为我们的图床

具体如何搭建，请见我的博客：(大家不要担心使用阿里云oss对象存储要花销很多钱，不需要的，如果只作为图床使用，是非常便宜的，每月资费不到1元哈哈，没听错，就是没到1元😂)

https://blog.csdn.net/weixin_39246554/article/details/112597337

![image-20211203161034887](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211203161034887.png)

好了，以上就是如何打造一款最强王者云笔记"typora+坚果云+阿里云oss"，大家赶快去使用吧！

## 此种方式云笔记的优缺点

### 1.优点

#### :round_pushpin: typora md编辑体验--王者(其它都是渣渣)

`typora`真的是贼几把太好用了，其他的编辑器、阅读器都是垃圾；

#### :round_pushpin: 图床使用阿里云oss(数据安全可靠，价格低廉，使用方便)

阿里云oss数据安全性是有报障的，并且资费也是非常低的；

啥时候typora可以提供图床功能了，那就贼几把赞了，其实现在有阿里云oss图床，已经能够满足要求了；

#### :round_pushpin: 自己要持续探究typora工具的使用

自己要对typora软件非常熟悉，对markdown语法要非常熟悉，对css要非常熟悉，这样我就可以继续定制我的typora主题了(这个功能真的是无敌了)；

![image-20211202105036225](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202105036225.png)

#### :round_pushpin: 数据迁移方便，且可方便同步文章到其他博客

typora笔记可以轻松导出各种格式，且迁移数据很方便；且可以一次上传到自己的hexo博客；

md软件结合各种云，转移都很方便。（这个非常关键，如果把维护数据都放在类似有道云等云笔记上去的话，迁移数据是非常麻烦的；因此采用坚果云+typora维护数据是非常完美的；）有道云和印象笔记，深陷进去，转出去就比较难了。

#### :round_pushpin: 坚果云的同步及其它功能是真的优秀

坚果云的同步功能非常不错，是文件级别的同步，保证了数据的完整性；同步完的状态从下面图标或者目录图标可以直观发现。

上传下载速度快；

坚果云笔记空间足够大，付费空间 30G，年付加享空间1G/月=每年12G

坚果云vip 199元/年；

书签功能不错；

注意：坚果云这种数据是直接存放在本地目录的，因此这些等待上传的数据可以随时更改数据，对上传不影响的，这个用户体验很不错。（2021.2.21）

### 2.缺点

#### 📍 typora左侧文档树功能默认不识别其他文件(已有解决办法)

typora默认新建的文件就是md，因此在使用`typora左侧文档树视图`功能时，同时想在某个目录下存放其他格式的文件，可以在其目录上打上一个tag。

不识别`.pdf  .sh`文件；

可以识别：`目录  .txt   .md`; 2021年12月4日17:34:00update

![image-20211202105604806](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202105604806.png)

![image-20211202105619121](https://bucket-hg.oss-cn-shanghai.aliyuncs.com/img/image-20211202105619121.png)

## 
