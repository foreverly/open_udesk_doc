# 放弃排队查询

 用于取得放弃排队的用户信息

 **重要:接口遵循** <http://www.udesk.cn/website/doc/apiv2/intro/>

## 请求

  GET /open_api_v1/im/im_queues.json

## 参数

```yaml
start_time: "2017-12-05 00:00:00"
end_time: "2017-12-06 00:00:00"
page: 1
per_page: 30 // 默认30
```

## 返回

```yaml
code: 1000
shut_queues:  // 内容为数组
    -
    customer_id: id
    customer_name: 用户匿称  
    channel: web // 渠道, web wechat ios android weibo api mchat
    queue_start_time: '2017-11-10T09:55:05.000+08:00' //开始排队时间
    queue_seconds: 104 //排队时间
    queue_name: '公司' //排队队列名
current_page: 1  // 当前页数
total_pages: 2   // 总页面
count: 200 // 当页总数?
```