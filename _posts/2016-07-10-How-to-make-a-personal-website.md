---
layout: post
title: "怎样制作个人网站"
published: true
---

以Bootstrap为框架制作在线简历/个人博客：

1.在官方网站：www.github.com上注册一个账号。
2.在github上新建一个仓库，创建个人站点。
3.下载并安装git软件，并以此配置SSH生成密钥，具体过程如下：
  打开Git Bash，输入命令：
  $ ssh-keygen -t rsa -C "youremail@example.com"
  在用户主目录里找到.ssh目录，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露出去，id_rsa.pub是公钥
  登陆GitHub，打开“Account settings”，“SSH Keys”页面，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容（即公钥）
  根据GitHub的提示，在本地的learngit仓库下运行命令：
  $ git remote add origin git@github.com:xumiao1994.github.io/cqc.git
  注意，把上面的 cqcre 替换成你自己的GitHub账户名
  下一步把本地库的所有内容推送到远程库上：
  $ git push -u origin master
4.选择合适的语言（我选择的是eclipse Java 1.7）在本地建立一个web工程并编写简历。
5.通过git软件将简历作为网站的主页上传并部署到仓库中，具体过程如下：
  在文件夹下打开Git Bash，输入以下命令：
  git add .
　git commit -m 'first_commit'
  git remote add origin https://github.com/findingsea/myRepoForBlog.git
　git push origin master
6.建立一个分支，利用Github Pages + Jekyll建立博客，用git将本地的博客文件上传并部署到新建的分支中，上传步骤如下：
  打开Git Bash，输入以下命令切换到你想放置本地代码仓库的位置：
  $ cd {本地路径}     // 比如：cd xmblog
  在Bash中依次执行以下三个命令完成文件的上传：
  $ git add .
  $ git commit -m "statement"   //此处statement填写此次提交修改的内容，作为日后查阅
  $ git push origin gh-pages
7.将博客链接到主页上。

<embed src="http://player.youku.com/player.php/Type/Folder/Fid/27614665/Ob/1/sid/XMTYzNzY5MDU0OA==/v.swf" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" allowFullScreen="true" mode="transparent" type="application/x-shockwave-flash"></embed>

[www.shipin.com](http://v.youku.com/v_show/id_XMTYzNzY5MDU0OA==.html?f=27614665&from=y1.3-idx-beta-1519-23042.223465.4-1#paction)




