---
title: How to use Hexo
tags: Hexo
---

# 安裝
:::info
安裝需求
檢查電腦是否已經安裝下列軟體：
* Node.js(Node.js 版本需不低於8.10，建議使用 Node.js 10.0 及以上版本)
* Git
:::
```shell=
# 安裝
npm install -h hexo-cli
```
<!--more-->
# 建立Hexo
```shell=
hexo init myBlog
cd myBlog
npm install
```
建立完成後，專案資料夾會有下列檔案：
```
.
├── _config.yml
├── package.json
├── scaffolds
├── source
|   ├── _drafts
|   └── _posts
└── themes
```

# Hexo 指令
## new
```shell=
hexo new [layout] <title>
```
建立一篇新的文章。如果沒有設定 layout 的話，則會使用 _config.yml 中的 default_layout 設定代替。如果標題包含空格的話，請使用引號括起來。
## generate
```shell=
hexo generate
```
產生靜態檔案。


| 選項 | 描述 |
| -------- | -------- |
| -d, --deploy     | 產生完成及部署網站     |
| -w, --watch     | 監看檔案變更     |

## publish
```shell=
hexo publish [layout] <filename>
```
發表草稿。
## server
```shell=
hexo server
```
啟動伺服器，預設是 http://localhost:4000/。

## deploy
```shell=
hexo deploy
```
部署網站。
| 選項 | 描述 |
| -------- | -------- |
| -g, --generate	     | 部署網站前先產生靜態檔案     |

# 基本操作
# 寫作
## 建立第一篇新文章

``` bash
$ hexo new [layout] <title>
$ hexo new post BasicConfig
```
### Layout
Hexo 有三種預設佈局：post、page 和 draft，它們分別對應不同的路徑，而您所自定的其他佈局和 post 相同，都儲存至 source/_posts 資料夾。


###### 官方資料
[Writing](https://hexo.io/docs/writing.html)
[Server](https://hexo.io/docs/server.html)
[Generating](https://hexo.io/docs/generating.html)
[Deployment](https://hexo.io/docs/one-command-deployment.html)

[Asset Folders](https://hexo.io/docs/asset-folders)
###### 參考資料
[NexT Theme for Hexo](https://theme-next.js.org/)
