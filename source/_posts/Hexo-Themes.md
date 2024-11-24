---
title: Hexo-Themes
date: 2024-01-18 23:18:34
tags:
    - Hexo
categories:
    - Hexo
---

# 安裝Hexo NexT主題
打開Terminal，進入資料夾並且安裝NexT theme。
```
$ cd <hexo-site>
$ npm install hexo-theme-next
```
<!--more-->
# NEXT Theme 設定(_config.yml)

## 背景顏色(白或黑)
背景顏色，黑色設定true，白色設定false。
```yml
# Dark Mode
darkmode: true
```
## 主選單Menu
```yml
menu:
  home: / || fa fa-home
  about: /about/ || fa fa-user
  tags: /tags/ || fa fa-tags
  categories: /categories/ || fa fa-th
  archives: /archives/ || fa fa-archive
  #schedule: /schedule/ || fa fa-calendar
  #sitemap: /sitemap.xml || fa fa-sitemap
  #commonweal: /404/ || fa fa-heartbeat

# Enable / Disable menu icons / item badges.
menu_settings:
  icons: true
  badges: false
```
## 主選單個人資料icon
放置圖片路徑
```
next/source/images/xxx.png
```
```yaml
# Sidebar Avatar
avatar:
  # Replace the default image and set the url here.
  url: #/images/avatar.gif
  # If true, the avatar will be displayed in circle.
  rounded: false
  # If true, the avatar will be rotated with the cursor.
  rotated: false
```
## 閱讀全文 More
首頁按鈕點進去，一般預設是可以文章全部內容，這邊介紹NexT其中一種方式可以顯示「閱讀全文」按鈕選單。
你的posts文章，可以選取你要的行數進行文章內容截斷
### 語法
```
<!--more-->
```
### 範例
```
# 安裝Hexo NexT主題
打開Terminal，進入資料夾並且安裝NexT theme。
<!--more-->
# NEXT Theme 設定(_config.yml)

## 背景顏色(白或黑)
背景顏色，黑色設定true，白色設定false。
```
###### 官方資料
[NexT Theme for Hexo](https://theme-next.js.org/)
###### 參考資料
