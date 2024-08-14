# 1.介绍
这是一个采用vercel进行部署typecho的Serverless项目。
# 2.如何使用？
将这个仓库star，并fork。在vercel里新建项目，选择这个项目，等待部署。并在vercel storage下新建一个Postgres Database。然后不出所料就会得到以下数据![一个包含数据库信息的东西](https://pic.imge.cc/2024/08/14/66bc2758a6c4a.jpg)
打开Show secret，default冒号后@前即为数据库密码
而@后面:5432前面为数据库地址。
打开vercel绑定的域名，在后面添加/install.php，填写数据库信息，类型为pgsql数据库用户名即为default，数据库名为verceldb
然后会生成config.inc.php文件内容，复制下来，放到新建的config.inc.php里，上传到你fork的仓库根目录，等部署完成后点继续，会填写一下信息，填写完后就可以享受你的typecho啦
# 3.常见问题
## 1.域名无法访问
请绑定自己的域名，vercel自带域名被墙了
## 2.数据库无法连接
请检查信息填写是否正确
## 3.怎么安装主题和插件
把插件或主题文件复制到usr/plugins或usr/themes目录下