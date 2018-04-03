# 操作指令

## init
> hexo init [folder]

建立一個新的網站。

## new
> hexo new [layout] \<title\>

建立一篇新的文章，如果沒有設定 layout 的話，則會使用 _config.yml 中的 default_layout 設定代替指定預設佈局，預設為 post；如果標題包含空格的話，請使用引號括起來。

### 佈局
Hexo 有三種預設佈局：post、page 和 draft

它們分別對應不同的路徑，而您所自定的其他佈局和 post 相同，都儲存至 source/_posts 資料夾。

|   佈局   |       路徑        |
|---------|:-----------------:|
|  post   |   source/_posts   |
|  page   |       source      |
|  draft  |   source/_drafts  |

## generate
> hexo generate

產生靜態檔案。

|   選項   |      縮寫      |        描述         |
|----------|:-------------:|--------------------:|
| --deploy |      -d       |  產生完成即部署網站  |
| --watch  |      -w       |     監看檔案變更     |

## publish
> hexo publish [layout] \<filename\>

發表草稿。

## server
> hexo server

啟動伺服器，預設是 [http://localhost:4000/](http://localhost:4000/)。

|   選項   |  縮寫  |          描述           |
|----------|:-----:|------------------------:|
|  --port  |  -p   |      覆蓋連接埠設定      |
| --static |  -s   |      只使用靜態檔案      |
|   --log  |  -l   | 啟動記錄器或覆蓋記錄格式  |

## deploy
> hexo deploy

部署網站。

|    選項    |  縮寫  |          描述           |
|------------|:-----:|------------------------:|
| --generate |  -g   |  部署網站前先產生靜態檔案 |

## render
> hexo render \<file\> [file2] ...

渲染檔案。

|    選項    |  縮寫  |   描述   |
|------------|:-----:|---------:|
|  --output  |  -o   | 輸出位置 |

## clean
> hexo clean

清除快取檔案 (db.json) 和已產生的靜態檔案 (public)。

## list
> hexo list \<type\>

列出網站資料。

## version
> hexo version

顯示版本資訊。