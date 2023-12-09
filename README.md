# psub
利用CF Worker搭建的反代订阅转换工具，通过随机化服务器地址和节点账号密码，解决用户转换订阅的隐私问题

### 演示网站
https://psub.888005.xyz

### 视频教程
https://youtu.be/X7CC5jrgazo

环境变量名：`BACKEND`

KV或R2变量名：`SUB_BUCKET`

### 参数
指定后端地址
&bd=https://api.v1.mk               # 肥羊增强，支持vless+hysteria订阅转换
&bd=https://sub.d1.mk               # 肥羊备用，支持vless+hysteria订阅转换
&bd=https://api.tsutsu.one          # 肥羊负载均衡
&bd=https://sub.id9.cc              # 品云，容易出现问题，不推荐
&bd=https://v.id9.cc                # 品云实验
&bd=https://id9.cc                  # 品云备用
&bd=https://sub.maoxiongnet.com     # 熊猫备用
&bd=https://pub-api-1.bianyuan.xyz  # 边缘

指定是否修改default-nameserver地址，主要配合mosdns实现防止dns污染与泄露
&regex=1                            # 启动后将默认dns地址设置为127.0.0.1

指定log-level
&loglevel=silent                   #silent, error, warning, info, debug

指定mixed-port，请自行校对，莫冲突
&mixedport=7890
&socksport=7891
&httpport=7892


### 支持反代转换的协议
 - shadowsocks
 - shadowsocksR
 - vmess
 - trojan
 - vless(取决于后端)
 - hysteria(取决于后端)

### 打赏
请我喝矿泉水：[全专线中专机场AFF链接](http://b.880805.xyz/)

请我喝桶装水：[搬瓦工美国CN2 GIA线路AFF链接](https://bwg.880805.xyz/)
