---
title: hexo架站
date: 2024-05-24 09:41:53
tags: hexo
excerpt: Hexo 靜態blog的建置
---

## 一、環境建置
```
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```

## 二、預設主題clone
* [landscape](https://github.com/hexojs/hexo-theme-landscape)
```
git clone --depth 1 https://github.com/hexojs/hexo-theme-landscape themes/landscape
```

## 三、基本指令操作
```
hexo clean  //清除快取
hexo s      //建立本地預覽
hexo g      //編譯
hexo d      //上傳

hexo new [title]         //建立文章
hexo new page [title]    //建立頁面
```


## 四、部署
1. 安裝 hexo-deployer-git
```
npm install hexo-deployer-git --save
```
2. 修改_config.yml設定
```
deploy:
  type: git
  repo: <repository url> #https://bitbucket.org/JohnSmith/johnsmith.bitbucket.io
  branch: [branch]
  message: [message]
```