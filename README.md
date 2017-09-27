# Webpack Deploy Markdown Site

Blog Framework built with node 6.0 +, Webpack, Vue 2.x, hexo-front-matter, markdown, visit [about](http://zaishanda.com/about).


## Instruction

In root doler, copy `.config-example.json` to `.config.json`, config params base on your machine.

`.config.json` 字段说明
 
 - markdownPath: 本地 markdown 的绝对路径
 - hash-deploy-url: 网站部署新版本的地址
 - public-url: qiniu cdn 图片地址
 - markdown-media-url: markdown 里面的图片资源保存位置

```
{
  "markdownPath": "/Users/someone/Documents/blog-markdown",
  "hash-deploy-url": "http://zaishanda.com:8081/?newhash=",
  "public-url": "http://__qiniu_cdn_domain__/site/",
  "markdown-media-url": "http://__qiniu_cdn_domain__/site-media/"
}
```

## Dir Instruction

 - data/bin 开发与部署时编译打包数据的脚本
 - data/build 和 data/build-dev 开发与部署数据编译打包结果
 - data/client-h5.js 客户端数据接口
 - build webpack 编译结果
 - src blog 网站页面代码


## 开发与部署 命令

### dev

`npm run dev` 进入开发模式


### build

`npm run build` 部署