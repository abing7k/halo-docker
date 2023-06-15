# halo-railway

单dockerfile，基于railway搭建halo个人博客

# 使用
请点击下方

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tqHt9L?referralCode=KQGLcx)

点击 deploy now

建议勾选 Private repository 因为涉及到自己数据库用户名密码及admin账户密码

# 创建完成

## 修改数据库链接为mysql
点击创建的halo-railway实例 ，进入setting，点击Source Repo进入github fork的仓库

点击创建的mysql 点击 connect

将MYSQL_URL替换 application.yaml 的 spring.r2dbc.url中的{MYSQL_URL}

将MYSQL_URL粘贴到 application.yaml 的 spring.r2dbc.username

将MYSQL_URL粘贴到 application.yaml 的 spring.r2dbc.password

## 修改管理员初始：

进入dockerfile

 修改--halo.security.initializer.superadminusername=你的管理员账户

 --halo.security.initializer.superadminpassword=你的管理员密码

## 修改完成：服务会自己重启 enjoy

