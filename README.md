## 爬虫  
>慕课网Go语言课程后面的爬虫项目  

* 爬取珍爱网数据


使用前需要安装  

ElasticSearch

```
//运行  如果没有elastic 将会拉取(需要科学上网或者更改docker镜像源)  -d 后台运行  -p 指定端口映射
docker run -d -p 9200:9200 elasticsearch
```

ElasticSearch Client

```
go get gopkg.in/olivere/elastic.v5
```  

一些需要的go包  
```
go get golang.org/x/net
go get golang.org/x/text
```


### 使用

* 首先运行 elasticsearch

* 运行main.go 爬取数据，存到elastic里

* 运行 frontend/start.go  启动web服务


在浏览器输入 自己的ip地址  即可访问