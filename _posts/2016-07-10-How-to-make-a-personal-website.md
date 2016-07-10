---
layout: post
title: "怎样制作个人网站"
published: true
---

以Bootstrap为框架制作在线简历/个人博客：

1.在官方网站：www.github.com上注册一个账号。</br>
2.在github上新建一个仓库，创建个人站点。</br>
3.下载并安装git软件，并以此配置SSH生成密钥，具体过程如下：</br>
  打开Git Bash，输入命令:</br>
  $ ssh-keygen -t rsa -C "youremail@example.com"</br>
  在用户主目录里找到.ssh目录，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露出去，id_rsa.pub是公钥</br>
  登陆GitHub，打开“Account settings”，“SSH Keys”页面，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容（即公钥）</br>
  根据GitHub的提示，在本地的learngit仓库下运行命令:</br>
  $ git remote add origin git@github.com:xumiao1994.github.io/cqc.git</br>
  注意，把上面的 cqcre 替换成你自己的GitHub账户名</br>
  下一步把本地库的所有内容推送到远程库上：</br>
  $ git push -u origin master</br>
4.选择合适的语言（我选择的是eclipse Java 1.7）在本地建立一个web工程并编写简历。</br>
5.通过git软件将简历作为网站的主页上传并部署到仓库中，具体过程如下：</br>
  在文件夹下打开Git Bash，输入以下命令：</br>
  git add .</br>
　git commit -m 'first_commit'</br>
  git remote add origin https://github.com/findingsea/myRepoForBlog.git</br>
　git push origin master</br>
6.建立一个分支，利用Github Pages + Jekyll建立博客，用git将本地的博客文件上传并部署到新建的分支中，上传步骤如下：</br>
  打开Git Bash，输入以下命令切换到你想放置本地代码仓库的位置:</br>
  $ cd {本地路径}     // 比如：cd xmblog</br>
  在Bash中依次执行以下三个命令完成文件的上传：</br>
  $ git add .</br>
  $ git commit -m "statement"   //此处statement填写此次提交修改的内容，作为日后查阅</br>
  $ git push origin gh-pages</br>
7.将博客链接到主页上。</br>

<embed src="http://player.youku.com/player.php/Type/Folder/Fid/27614665/Ob/1/sid/XMTYzNzY5MDU0OA==/v.swf" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" allowFullScreen="true" mode="transparent" type="application/x-shockwave-flash"></embed></br>

[www.shipin.com](http://v.youku.com/v_show/id_XMTYzNzY5MDU0OA==.html?f=27614665&from=y1.3-idx-beta-1519-23042.223465.4-1#paction)




