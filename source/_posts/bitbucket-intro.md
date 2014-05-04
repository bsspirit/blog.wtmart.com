title: bitbucket简单使用介绍
date: 2013-06-16 02:30:43
author: Dan Zhang
categories:
- IT技术
tags:
- bitbucket
- git
---

**bitbucket注册账号**

bitbucket.org，要翻墙

**登陆server3系统**

    ssh zd@desk3.wtmart.com -p 10001

**生成密钥**

    ssh-keygen -t rsa -C "bsspirit@163.com"

**复制公钥**

```{bash}
cat ~/.ssh/id_rsa.pub
ssh-rsa EFWzaC1yc2EADSGEDBAAABAQCekoni4TRTQ7/EcrPiUCoU8lP/4wRseWMOW6GFRL10JXmhPHC5EU0BB+tHgPZ/lCzJMfkEECFcv6R4Nzgx41GUcu18ANdz22TP/ovSa+248jFkH9wq3aXVOTlW/ce+XDrJiVQC1CVjGbX61Au9zeNhMO/DTCg88zSeufXbOsTUyCpezGZST7NHM6ubpl/C81ey9I9TodRKDKNVIOSffi2RbulaHKirim9olo7zodfm3ISeMZC7C0MPZw8y8V00zzeBNWOqWfsXhaAP8ft1LFLaWsEn2rhyGM3TRT1i/pgC5xNLYKAQz0FYhzx1fWRnrRgj4ub6iMRjlCNcLy3oBIMx xxx@server3
```

**配置到bitbucket自己的账号里面**
头像--&gt;manage account--&gt;SSH keys--&gt;add

**下载代码：（在lin.wtmart.com的环境中，请使用copy的方法。）**

    git clone git@bitbucket.org:bsspirit/cosinvestment.git

由于网络不稳，要试十几次才能下载成功。(可以直接从主目录copy一份，也可以用，请COPY方法)

另一种https的方式（翻墙），这里不建议用（git clone https://bsspirit@bitbucket.org/bsspirit/cosinvestment.git）

**copy的方法：**

    scp git@git.wtmart.com:/home/git/repo/a.tar.gz .

**密码git**

    tar xvf a.tar.gz
    cd cosinvestment/
    git pull

**做第一次提交：**

    vi a.txt
    修改点什么

    git add .
    git commit -m 'xxx update test'
    git push -u origin master