title: 在Github上写R包
date: 2013-08-04 05:30:56
author: deng yishuo
---

申请 Github 账号之后就可以在 Github 上与朋友协助写 R 包了。写 R 包的步骤大致如下：

建立一个以包名，比如，quanttools 命名的库（repository），最简单的方法是登录github，并在个人主页上，点击右上角的 creat a new repo 创建新的库。

打开本地的 git ，键入 git clone https://github.com/dengyishuo/quanttools.git  即可把新建的库复制到本地的 git 路径下，对应的文件夹名为 quanttools 。

用 package.skeleton 函数生成 R 包的骨架，将整个骨架原封不动复制到 quanttools 文件夹中即可。

运行

git add .

git commit -am "some annotation"

git push

把更改的 quanttools 文件夹更新到 github 端。

如果有任何需要更新的文件，只需要在本地文件夹中进行新建、编辑和修改，然后，运行上面的三个命令，即可对包的内容尽心更新。

多人协作时，还需要 git pull ，即把本地端与 github 端进行同步。比如，Newton2 对 quanttools 的 R 文件夹进行了修改，bsspirit 最好现在本地端运行 git pull 将Newton2 更新的文件夹同步到本地，再在本地对相应的文件进行更改、编辑等。否则，需要运行 git merge 来合并各个分支。

还有一种简单的方法，是直接在 github 端对文件进行在线编辑，此时，需要登录 github ，找到需要编辑的文件路径，点开，点击右上角的 edit 选项卡，即可进入文件编辑模式，此时，可对文件进行相应的修改。修改完毕，需要点击下面的 commit 按钮来提交修改。每次提交修改时，最好写清楚提交注释，便于其它人知道每次提交动作都做了哪些修改。
