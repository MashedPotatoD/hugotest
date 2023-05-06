---
title: "Blog搭建之路"
date: 2023-05-05T22:13:17+08:00
draft: false
---
[TOC]


# <span style="color:cyan;">一起搭建一个超级炫酷的blog吧:smile:</span>

<span style="color:magenta;">
写在前面: 搭建过程基本基于官方文档
</span>

## 1.在本地搭建hugo站点
- 官方文档:[本地建站](https://gohugo.io/getting-started/quick-start/)
- 注意事项:
    - draft: true代表这个.md文件是草稿，在使用hugo命令（会在public目录下生成所有的静态文件，这些文件最终在网页上展示，必须提交，而hugo站点的根目录的其他文件其实可以不用提交）发布站点时不会发布草稿文件，如果需要发布那应该将值改为true。
	- 站点配置文件config.toml中的baseurl可以等到部署后再修改
    - 本地部署成功之后访问localhost：1313，服务器开启时在本地改动md文件并保存浏览器会立马更新内容。部署到github上之后就不会了，需要把更新内容推送到github。

## 2.将站点部署到github上
- 官方文档:[部署到github](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
- 注意事项:
    - 将本地存储库推送到github时要注意，每个仓库都有一个分支，也可以理解为大仓库里的小仓库，要推送过去，不仅要跟线上远程仓库有关联，还要跟线上远程仓库的某个分支关联。步骤大概如下：
        1. 初始化仓库: `git init`
        2. 检查仓库状态是否有变: `git status`
        3. 提交本地版本库: `git commit -m "msg"`
        4. 将本地分支命名为main: `git branch -M main`
        5. 关联本地仓库和远程仓库: `git remote add origin 仓库url`
        6. 关联分支: `git pull --rebase origin 分支名`
        7. 推送: `git push -u origin main`
    - 以上步骤只有推送到远程仓库这一步是需要联网进行的，其余都在本地，而这一步很容易受到网络影响，如果不开代理经常不成功；开了代理端口会变，尽量在进行这一步时保证代理中的主机只有443端口，删除其他端口的主机。

## 3.其他的参考资料
- [别人的搭建经验](https://pingfan.me/posts/cs/create_blog_with_zero_experience/)
- 对blog进行功能增强
    - [文字教程](https://leftpocket.cn/post/hugo/hugo_vercel/)
    - [视频教程](https://www.youtube.com/watch?time_continue=5&v=ruSga8MVRKA&embeds_euri=https%3A%2F%2Fleftpocket.cn%2F&source_ve_path=Mjg2NjY&feature=emb_logo)

#### *做到这里就大功告成啦~*:wink: