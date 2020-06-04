# html-i18n-cli

> HTML 国际化工具

## 安装

``` sh
1. 安装 Node.js

2. npm install 

3. 安装 yarn 代替 npm （可选）
npm i -g yarn 

```

## 使用

1. 生成 JSON 文件

``` sh
npm run parse test/test.html

// yarn parse test/test.html
```

2. 翻译 JSON 文件

> 输入两次 Ctrl + C 终止，机翻后可手动校对

``` sh
npm run trans test/test.json -t en

// 或 yarn trans test/test.json -t en
```

  * -t zh 指定[目标语言](http://api.fanyi.baidu.com/doc/21)
  * -n 50 指定更新频率

3. 还原 HTML 文件

``` sh
node ./bin/html.js render test.html test.json
```

## 附加功能

* JSON 转 EXCEL

``` sh
node ./bin/html.js convert test.json
```

* EXCEL 转 JSON

``` sh
node ./bin/html.js convert test.xlsx
```
