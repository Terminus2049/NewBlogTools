# NewBlogTools
整理独立博客/网站、具备公共备份功能的工具。

## 为什么要建立独立博客/网站

### 创建独立博客/网站的成本低到难以想象

最重要的写在最前面。

现在市面上有非常多的建站工具，而且对小白用户非常友好，不需要任何计算机知识就能搭建一个独立网站。比如基于 GitHub Page 的博客/网站，不仅不需要购买、架设服务器，而且能够多人协作，哪怕是陌生人。许多大型的中文文档就是基于 GitHub 来完成的，比如 [TensorFlow-zh](https://github.com/jikexueyuanwiki/tensorflow-zh)。

### 建立独立品牌，减少封禁损失

微信既能删除素材，也能封禁帐号。帐号被封禁意味着所有努力归零。拥有一个独立网站，可以大大减少被微信删除或者封禁的损失。即使你的公众号没有这种危险，拥有一个独立网站，也能更好地传播和建立自己的品牌。此外，如果你的文章常常被删除，可以直接推送独立博客中的文章链接，这样不仅被删的机率大大减小，即使在链接被微信阻止访问后，仍能通过复制到浏览器打开。要知道微信不能仅凭一个链接就能通过算法进行过滤，而且要知道，是公众号作者的辛勤码字为微信提供了过滤算法的素材。

关于这一点，[湾区日报](https://wanqu.co/about/) 是一个不错的案例，虽然这个博客分享的内容偏技术类，而且也有微信订阅号，但其推送方式与其他的博客不同，他的微信订阅号每次只推送博客的文章题目和链接，而不是用微信订阅号图文消息。

在这里必须推荐一下「政见」（<http://cnpolitics.org/>）和大象工会。当然你也可以了解一下王五四的故事。看看这些大号是怎么做的。

### 公共备份和可检索性

许多人把文章仅仅发布在微信公众号、微博或者豆瓣日记这样的平台。微信公众号文章是不能被搜索引擎收录的，这意味着用户使用关键词搜索是不可能看到你的文章。要知道用户的关键词主动搜索意味着这名用户与文章受众的强烈吻合，不要失去你的目标用户！

另外，把文章发布在豆瓣这样的平台，豆瓣有可能将其转为仅作者可见。而且豆瓣审核通过才公开可见，搜索引擎也无能为力。现在，不仅是私有平台搜索引擎无法访问，哪怕是搜索引擎可访问的非独立平台，现在删贴技术已十分发达，在搜索引擎收录前就已经删除。

我相信作者手里肯定有文章备份，但你保存在 pocket/印象笔记里的备份，其他用户只能通过直接链接访问，而不能通过检索得到。这极大地限制了二次传播。博客和独立网站是能够被搜索引擎收录的，是一种公共备份，是最优的选择。其次是 <http://archive.is/> ，用户虽然不能检索，但是可以直接去 <http://archive.is/> 上查看所有的备份文章，例如 <https://archive.is/mp.weixin.qq.com> 可以查看所有的微信公众号备份。遗憾的是 <http://archive.is/> 没有提供标题检索的功能，但这一功能是非常容易开发的。当然，你不必了解这些细节。

## 写给小白的建站指南

### 基于 GitHub Page（推荐）

GitHub Page 无需购买主机，甚至不需要额外购买域名，而且还能协作，还能抗封锁，不知道比 WordPress 高到哪里去了。

搭建 GitHub Page 最简单的方法是 Fork 一个已有的站点，比如 <https://github.com/TerminusBot/terminus-jekyll-template>。

只需要以下几个简单的步骤：

1. 注册 GitHub
2. fork https://github.com/TerminusBot/terminus-jekyll-template
3. 在 Settings 中打开 GitHub Page，source 选择“master branch”
4. 在 Settings 中修改项目名称，如 Blog（或者其他任何英文名称），然后你就可以在 `https://yourusername.github.io/blog` 看到你的网站。
5. 在about.md文件中修改个人简介，在 _config.yml文件中修改网站名和网站简介。
6. 按照 _posts 文件夹中的格式写文章，新文章以yyyy-mm-dd-engligh-title.md 的格式命名，放在 _posts 文件夹下。

你可以在 <http://jekyllthemes.org/> 尽情挑选你觉得最好看的主题。

### 新手友好工具

[gridea](https://github.com/getgridea/gridea): 一个静态博客写作客户端
[HUGO](https://gohugo.io)：采用 go 开发的 HUGO 引擎，渲染速度更快，教程 [Using Hugo, GitLab Pages, and Cloudflare to create and run this Website](https://tkainrad.dev/posts/using-hugo-gitlab-pages-and-cloudflare-to-create-and-run-this-website/)

### 基于 WordPress

略

## 实用工具

### 公共备份工具

* [ArchiveTeleBot](https://github.com/Terminus2049/ArchiveTeleBot) 自动存档网址的 Telegram 机器人
* [archive.is](http://archive.is/)：抓取能力强，可通过被删文的网址查找。（已被墙）
* [Internet Archive](https://archive.org/)：互联网档案馆（已被墙）
  * [save-to-the-wayback-machine](https://verifiedjoseph.com/projects/save-to-the-wayback-machine)：互联网档案馆的插件

### 迁移工具

* [蜜蜂采集-BeePress](https://wordpress.org/plugins/beepress/)：将微信公众号、今日头条、简书、知乎专栏文章导入 WordPress。

## 其他建议

希望您能给原创文章添加 cc 协议，关于 cc 协议建议读读阮一峰的博文[谈谈创作共用许可证（Creative Commons licenses）](http://www.ruanyifeng.com/blog/2008/04/creative_commons_licenses.html)。
