分布式美团外卖小爬虫 ，利用RabbitMQ消息队列
===
### 小说明

* 第一次比较大的在github写一个项目，一切都在摸索中。当然这个项目也是第一次接触分布式爬虫。<br>
* 整体思路是RabbitMQ+多实例+多线程搞定。
* 预期目标是，美团数据在2个小时内完全抓取完（这个时间是我瞎定的，美团对于IP的限制太可怕了。<br>
* IP这里我用的是<a href ="https://www.abuyun.com/">阿布云</a>）	<br>
* 具体实现方式和具体处理，还在摸索中......，如有大神路过还望指点....

## 目前进度：

* 获取美团全国城市列表，并以JSON格式添加到远程RabbitMQ服务器队列<br>
* 从队列中获取城市列表，解析该城市美团店家分类<br>
* 添加网页处理类，用来解析各种分类的店铺
* 完善各种异常，
* 路漫漫其修远兮，吾将上下而求索


