这是COS Investment的官方博客
===============================

访问地址：http://blog.wtmart.com/.

博客基于hexo系统搭建在github上面，使用前需安装node和hexo。

### 安装系统环境

+ http://blog.fens.me/nodejs-enviroment
+ http://blog.fens.me/hexo-blog-github/

### 克隆项目库到本地

```{bash}
git clone git@github.com:bsspirit/blog.wtmart.com.git
```

### 创建一篇新文章

```{bash}
cd blog.wtmart.com
git pull
hexo new [layout] <title>
hexo new post new_post
```

###在本地查看启动服务器
```{bash}
hexo server
```

### 生成静态文章

```{bash}
hexo generate
```

### 发布到在服务器
```{bash}
hexo deploy
```

### 上传源文件

```{bash}
git add .
git commit -m "***"
git push
```
