# flask_bookstore
# 原项目
##### https://github.com/hyc-shayu/flask_bookstore


# 图书商城系统-网上书店

# 网站介绍  
游客可以浏览、搜索、查看图书，查看评论等  
登录用户可以 浏览 搜索 查看 图书，查看 发布 回复 评论，添加到购物车，收藏，添加收货信息，购买 使用支付宝支付、订单操作 等  
管理员 可以 管理 图书、订单、滚屏图片 等。  



# 数据迁移
###### 需要把映射到数据库中的模型导入到manage.py文件中，否则映射就不成功
step1(首次), 初始化环境：python manage.py db init 
###### 忽略提示　Please edit configuration/connection/logging settings in 

step2,自动检测模型 生成迁移脚本：python manage.py db migrate # 模型变化执行

step3,将迁移脚本映射到数据库中：python manage.py db upgrade


# 安装包
1. 用Bootstrap-Flask,不要用flask_bootstrap
2. mysql-connector-python-rf
3. flask_sqlalchemy版本3.0.2报错,降级2.5.0
