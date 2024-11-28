
### Laravel Admin CMS

基于Laravel 11的后台内容管理开发系统，后台基于layui-mini前端主题。能够帮助你节约开发基础系统功能，及一些常规功能插件。是一个快速上手，项目基础开发，外包开发首选CMS。

- 后台系统常用功能

- 支持主题风格设置`单页面`和`iframe多标签`

- 简单上手，快速开发

- 更多插件功能，一键安装扩展

- 完全开源，更好的进行业务开发

- 定期更新laravel主版本

整体功能待完善，欢迎`star`。


### 演示demo

- 地址：~~不再提供~~

- 账号：admin

- 密码：123456

- 演示说明：理性演示，误删除基础数据，可自行添加数据，自行删除（数据库会不定时重置抹除数据）


### 如何使用

- 使用前学习

  需对`laravel`有基础了解，以及简单开发经验

- 获取代码
```bash
cd path
composer install
```
- 配置数据库`.env`(如没有复制`.env.example`改名)
```bash
php artisan key:generate
```
- 删除所有表
```bash
php artisan migrate:fresh
```
- 数据库表迁移
```bash
php artisan migrate
```
- 基础数据信息填充
```bash
php artisan db:seed --class=InitSeeder
```
- 上传文件路径符号链接
```bash
php artisan storage:link
```
- 项目启动
```bash
php artisan serve
```

- 获取路由列表:仅显示以给定 admin/image_manager 开头的路由
```bash
php artisan route:list --path=admin/image_manager
```

- 格式化代码
```bash
php vendor/bin/php-cs-fixer fix
```
```bash
composer phpcs
```

- 生成ide辅助文件
```bash
php artisan ide-helper:generate
php artisan ide-helper:models
php artisan ide-helper:meta
```


- 项目访问

  后台地址：`http://127.0.0.1:8000/admin`

  后台账号：admin

  后台密码：123456（生产环境必须修改密码）


### 基础功能

- 用户管理

- 菜单管理

- 角色权限管理

- 配置管理

- 日志管理

- 插件管理

### 云存储支持

开启云存储后，在上传附件到本地后，同时上传一份到云存储位置，并获取云地址。

查看配置文件`gui.upload_driver`和`filesystems.disks.*`了解配置认证秘钥

- 阿里云：oss（[开通地址](https://www.aliyun.com/product/oss?userCode=hhlk0aji)）
- 七牛云：kodo（[开通地址，免费10G](https://s.qiniu.com/jyQv6v)）


## 界面截图
- 单页面效果

![image](public/preview/onepage.png)

- 多标签iframe

![image](public/preview/tab_iframe.png)

## 许可证

完全开源免费，请保留项目开源版权说明。本项目遵循开源协议 [MIT license](https://opensource.org/licenses/MIT).
