# 中文搜索 xunsearch Mac + Laravel5.1

## 安装

``` shell
wget http://www.xunsearch.com/download/xunsearch-full-latest.tar.bz2
tar -xjf xunsearch-full-latest.tar.bz2
cd xunsearch-full-1.4.9
sh setup.sh
```

## 启动 xunsearch

由于安装在 `/usr/local/xunsearch`，执行
`sh /usr/local/xunsearch/bin/sh xs-ctl.sh start|restart`

## composer下载Xunsearch PHP-SDK到Laravel中

``` shell
cd ~/sites/laravel
composer require --prefer-dist hightman/xunsearch "*@beta"
```

* # sdk目录结构

* ``` shell
hightman
└── xunsearch
├── README.md
├── app
│   ├── demo.ini
├── composer.json
├── lib
│   ├── XS.class.php
│   ├── XSDocument.class.php
│   ├── XSFieldScheme.class.php
│   ├── XSIndex.class.php
│   ├── XSSearch.class.php
│   ├── XSServer.class.php
│   ├── XSTokenizer.class.php
│   └── xs_cmd.inc.php
├── util
│   ├── Indexer.php
│   ├── IniWizzard.php
│   ├── Logger.php
│   ├── Quest.php
│   ├── RequiredCheck.php
│   ├── SearchSkel.php
│   ├── XSDataSource.class.php
│   ├── XSUtil.class.php
│   ├── skel
│   └── xs
└── wrapper
├── yii-ext
└── yii2-ext
```

## 命令行 体验demo使用

