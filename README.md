# 数据库设计

## 博客表

| id  | title | content | createtime    | author   |
| --- | ----- | ------- | ------------- | -------- |
| 1   | 标题-1  | 内容-1    | 1640874478457 | zhangsan |
| 2   | 标题-2  | 内容-2    | 1640874485070 | lisi     |

## 用户表

| id  | username | password | realname |
| --- | -------- | -------- | -------- |
| 1   | zhangsan | 123      | 张三       |
| 2   | lisi     | 123456   | 李四       |

# 接口设计

| 描述     | 接口               | 方法   | url 参数          | 备注                |
| ------ | ---------------- | ---- | --------------- | ----------------- |
| 获取博客列表 | /api/blog/list   | get  | author, keyword | 选择 url 参数可以按关键字查询 |
| 获取博客内容 | /api/blog/detail | get  | id              |                   |
| 新增博客   | /api/blog/new    | post |                 |                   |
| 更新博客   | /api/blog/update | post | id              |                   |
| 登录     | /api/user/login  | post |                 |                   |



# 登录

业界有统一解决方案，一般无需重新设计。
