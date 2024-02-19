# Scada Tool Api Gateway Service

本專案運用Krakend設定 Scada Tool Api 路由服務

## Prerequirement

- krakend:2.1.4

## 相關服務

+ [Auth service](https://github.com/muulinCorp/auth)
+ [Configuration service](https://github.com/muulinCorp/configuration)
+ [Storage service](https://github.com/94Peter/storage)

## 開發環境安裝

1. [install Docker](https://docs.docker.com/engine/install/)

## 專案目錄檔案資訊

| 名稱         | 類型      | 用途  |
| -----------  | --------- | ----- |
| doc          | 目錄      | 服務API文件 |
| partials     | 目錄      |  krakend partial tmpelate  |
| plugin       | 目錄      |  krakend外掛  |
| settings     | 目錄      |  krakend endpoint 對應 backend api  |
| krakend.tmpl | 文件      |  krakend範本  |

### partials說明
* [rate_limit_endpoint.tmp參考文件](https://www.krakend.io/docs/endpoints/rate-limit/)

### plugin說明
* static-filesystem.so
> 將路徑/doc/* 對應至目錄doc內的文件

[開發說明](https://www.krakend.io/docs/extending/)

### settings
* endpoint.json
> 設定服務Api路由清單
