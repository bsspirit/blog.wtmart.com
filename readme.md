COS博客
===============================

基于hexo系统搭建在github上面。

访问地址：http://blog.wtmart.com/

安装node,hexo

+ http://blog.fens.me/nodejs-enviroment
+ http://blog.fens.me/hexo-blog-github/

```{bash}
git clone git@github.com:bsspirit/blog.wtmart.com.git
```

创建一篇新文章

```{bash}
hexo new [layout] <title>
hexo new post new_post
```

在本地查看启动服务器
```{bash}
hexo server
```

生成静态文章

```{bash}
hexo generate
```

发布到在服务器
```{bash}
hexo deploy
```