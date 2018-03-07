# 客服消息

## 获取实例

```php
$service = $app->customer_service;
```

> 使用方法详看公众号-客服消息章节。

图文消息和公众号不同
```php
$service = $app->customer_service;
$message = new Link([
   'title' => 'xxx',
   'description' => 'xxx',
   'url' => 'https://www.easywechat.com/',
   'thumb_url' => ''
]);
$service->customer_service->message($message)->to($openid)->send();
```
