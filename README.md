# 讨论区编写指南
你可以在这里讨论数学问题，支持 Latex！你只需要把你的 Latex 代码复制过来！由于暂时不支持定理类环境，请花几分钟读一下[Markdown 基本语法](https://www.markdown.xyz/basic-syntax/#overview). 特别注意的是，在复制你的 latex 代码过来的时候，请用段落（Paragraphs），否则复制过来的 latex 代码会乱。 所有讨论区文章在当前仓库，即[Discussion](https://github.com/LanglandsLearningGroup/Discussion)中进行编写改动，请不要在[LanglandsLearningGroup.github.io](https://github.com/LanglandsLearningGroup/LanglandsLearningGroup.github.io)改动，否则会被覆盖掉。我提倡一个话题一个文件。在创作前请耐心仔细读完如下指南。

### 文件命名
讨论区的所有文件名必须为`YYYY-MM-DD-title.md`的格式。其中`YYYY-MM-DD`为日期，需要创建者手动填写。`title`是可以随意取的，方便你自己识别便可。一般可由英语字母，数字，下话题和短横线组成。**如果文件不符合上述命名规则，则不会被系统识别。**
### 文件元信息
讨论区的所有文件必须以以下代码开始：
```
---
layout: article
tags: discussion
title: Your Article Title
mathjax: true
permalink: your_link.html
author: Your Name
key: your_key123
---
```
每行含义如下：
* `layout`：本页布局。必须存在，请勿做任何改动。
* `tags`：本页标签。请勿删除`discussion`标签以免文件不显示在讨论区专栏。你也可以添加更多的tag。多个tag需要写成：
```
tags: [discussion, padic, rational, field]
```
另外每个tag中最好不要带空格。
* `title`: 本页的标题。你可以用英语，中文，甚至带LaTeX公式。这些都是支持的。
* `mathjax: true`：必须存在，请勿做任何改动。
* `permalink`: 可选，如不想填请删除本行。此博客系统默认会根据文件名中的日期来生成最后网页的路径。这不会引起任何问题，但有时候路径会看上去比较冗长，不太美观。`permalink`选项可以覆盖此网页路径的生成规则。简单来说，如果你想让此页的网址为`https://langlandslearninggroup.github.io/your_link.html`, 那么`permalink`此项就应该填成
```
permalink: your_link.html
```
* `author`: 可选。如果不想填请删除此行，这种情况下该页将会以Langlands纲领学习小组的名义发布。如果你想自己署名，请看以下`作者署名`部分。
* `key`: 如果想对此页开启评论功能，则该项必须填，否则可以删除该行。key必须由英语字母开头，由英语字母下划线和数字组成。

**注意**：以上`permalink`与`key`需要有唯一性，即不同的.md文件的`permalink`与`key`必须不同，否则会出错。
### 作者署名
如果你想自己让文章署上自己的名字，而不是以Langlands学习小组的名义发表，那么请先在[这里](https://github.com/LanglandsLearningGroup/LanglandsLearningGroup.github.io/blob/master/_data/authors.yml)填写你的个人信息。格式见此
```
Profile Name:
  name      : Your Name
  url       : #https://tianqi.name
  avatar    : #你的头像，应该是个指向图片的网址。如：https://avatars.githubusercontent.com/u/32867606?v=4
  bio       : #个人简介
  email     : #kitian616@outlook.com
  facebook  : # "user_name" the last part of your profile url, e.g. https://www.facebook.com/user_name
  twitter   : # "user_name" the last part of your profile url, e.g. https://twitter.com/user_name
  weibo     : # "user_id"   the last part of your profile url, e.g. https://www.weibo.com/user_id/profile?...
  googleplus: # "user_id"   the last part of your profile url, e.g. https://plus.google.com/u/0/user_id
  telegram  : # "user_name" the last part of your profile url, e.g. https://t.me/user_name
  medium    : # "user_name" the last part of your profile url, e.g. https://medium.com/user_name
  zhihu     : # "user_name" the last part of your profile url, e.g. https://www.zhihu.com/people/user_name
  douban    : # "user_name" the last part of your profile url, e.g. https://www.douban.com/people/user_name
  linkedin  : # "user_name" the last part of your profile url, e.g. https://www.linkedin.com/in/user_name
  github    : # "user_name" the last part of your profile url, e.g. https://github.com/user_name
  npm       : # "user_name" the last part of your profile url, e.g. https://www.npmjs.com/~user_name
```

注意：
* 填写时，请将以上内容复制一份粘贴到文件末尾进行修改，而不是直接在他人的资料上修改
* 你没有或者不想透露的个人信息就让它保持在被注释，即以#开头的状态即可。想填的请参考注释。
* 填完以后请把对应项的注释删掉，或者在注释和你填入的内容间插入一个空格。
* `Profile Name`也是需要改成你的名字的。
* 正如Yiqi Xu的信息，`Profile Name`和`name`可以相同，但也可以不同。最后在网页中显示的是`name`。但在你写的文章中，`author`项应该填入`Profile Name`的值。我没有测试，但`Profile Name`最好是英语的。

## 关于评论区
很遗憾，目前为止评论区还没有办法支持公式输入。而且在短时间内这种情况可能不会改变。目前比较好用的评论区有`Gitalk`和`Valine`两种。前者实际利用本仓库Issue区作为评论区。它的好处是你可以在Issue里看到每个帖子的讨论，配合浏览器插件能实现部分公式渲染；坏处是每个帖子的评论区需要管理员（目前是Yijun Yuan，可设为多人）手动开启。而`Valine`的好处是使用比较简单，支持游客评论，潜在支持MathJax（但我不知道怎么开启，可能无法开启）。
