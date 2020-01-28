# Hexo Baidu URL Submit

![百度主动提交](http://hui-wang.info/2016/10/23/Hexo%E6%8F%92%E4%BB%B6%E4%B9%8B%E7%99%BE%E5%BA%A6%E4%B8%BB%E5%8A%A8%E6%8F%90%E4%BA%A4%E9%93%BE%E6%8E%A5/baidu_urls_submit.png)

[开发动机和使用文档](https://www.hui-wang.info/2016/10/23/Hexo插件之百度主动提交链接/)

# 熊掌号支持

## baidu_url_submit 配置

| 参数     | 示例           | 说明                                        | 注意                                    |
| -------- | -------------- | ------------------------------------------- | --------------------------------------- |
| count    | 1000           | 提交最新的一个链接个数                      |                                         |
| host     | alili.tech     | 在百度站长平台中注册的域名                  |                                         |
| token    | xxxx           | **敏感信息**                                | 环境变量 BAIDU_URL_SUBMIT_TOKEN 获取    |
| path     | baidu_urls.txt | 文本文档的地址， 新链接会保存在此文本文档里 |                                         |
| xz_appid | xxxx           | **敏感信息** 熊掌号 appid                   | 环境变量 BAIDU_XZ_URL_SUBMIT_APPID 获取 |
| xz_token | xxxx           | **敏感信息** 熊掌号 token                   | 环境变量 BAIDU_XZ_URL_SUBMIT_TOKEN 获取 |
| xz_count | 10             | 从所有的提交的数据当中选取最新的10条        |                                         |

## deploy 配置
```
deploy:
- type: baidu_url_submitter # 百度
- type: baidu_xz_url_submitter # 百度熊掌号
```