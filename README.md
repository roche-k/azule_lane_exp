# 计算经验船效率的小工具

### 使用步骤

1. 下载

git clone https://github.com/roche-k/azure_lane_exp

2. 安装环境

例子：Deb系

sudo apt install python3 python3-pip
sudo pip3 install jupyter matplotlib numpy

3. 进入clone的文件夹，运行
jupyter notebook

4. 参照文档内的帮助文件，配置实际运行环境，运行整个文件

### 例子

练2艘航母，航母平均最大油耗13油  
用一个经验船，经验船加成15%，经验船油耗3油  
每次都是后排旗舰位的mvp

ship_oil = 13.0  
ship_number = 3  
ship_xp_number = 1  
ship_xp_oil = 3.0  
ship_xp_rate = 0.15  
ship_leader = 1  
mvp = 1.0  

练1艘轻巡，轻巡平均最大油耗11油  
用一个经验船，经验船加成16%，经验船油耗2油  
轻巡拿到mvp的概率为50%  

ship_oil = 11.0  
ship_number = 2  
ship_xp_number = 1  
ship_xp_oil = 2.0  
ship_xp_rate = 0.16  
ship_leader = 0  
mvp = 0.5

在文章末尾的显示图

横轴代表吃经验船的平均油耗，纵轴代表经验效率

绿色线代表不使用经验船，随着平均油耗增高，经验效率的变化情况  
红色线代表使用经验船，随着平均油耗增高，经验效率的变化情况

例如这里的图，表示  
在特定情况下，每船平均8.4油前，不使用经验船经验效率较高  
平均每船高于8.4油时，使用经验船效率较高

![oil](https://github.com/roche-k/azure_lane_exp/blob/master/oil.png)
