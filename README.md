## massa测试网v0.1.1 docker一键部署脚本（Ubuntu&CentOS）（支持多节点部署）
### ===本脚本仅限TopMininG社群用户使用===
#### ■ 一键脚本运行方法(整行复制粘贴执行)：
  
#### @国内用户：
##### ・Ubuntu：
##### ___`sudo apt update && sudo apt-get install wget curl`___
##### ・CentOS7：
##### ___`sudo yum update && sudo yum install wget curl`___
##### ・CentOS8：
##### ___`sudo yum update --nobest && sudo yum install wget curl`___
##### 
##### ___`wget https://gitee.com/topmininglabs/massa/raw/main/topmining_massa.sh.x && chmod +x ./topmining_massa.sh.x && sudo ./topmining_massa.sh.x`___
  
#### @海外用户：
##### ・Ubuntu：
##### ___`sudo apt update && sudo apt-get install wget curl`___
##### ・CentOS7：
##### ___`sudo yum update && sudo yum install wget curl`___
##### ・CentOS8：
##### ___`sudo yum update --nobest && sudo yum install wget curl`___
##### 
##### ___`wget https://github.com/topmininglabs/massa/raw/main/topmining_massa.sh.x && chmod +x ./topmining_massa.sh.x && sudo ./topmining_massa.sh.x`___
#####   

#### ■ 操作方法：
<img width="391" alt="スクリーンショット 2021-08-04 23 53 46" src="https://user-images.githubusercontent.com/86814869/128203556-6f219201-1998-47f4-845c-4c7236430eb3.png">


##### 1.输入选项1安装Docker
##### 2.输入选项2下载TopMininG专供massa镜像
##### 3.输入选项3运行massa容器节点(支持多节点部署)
##### 4 输入选项4进入节点钱包交互界面进行钱包操作和质押操作
##### 4.1.新建钱包（请保管好钱包地址和私钥）
##### ___`wallet_new_privkey`___
##### 4.2.查询钱包信息（请确保有足够的测试币，测试币通过最下方的官方Discord领取）
##### ___`wallet_info`___
##### 4.3.购买roll（购买一个roll需要500个币,fee可填0,购买完成大概1分钟左右可查询）
##### ___`buy_rolls <wallet_address> <roll count> <fee>`___
##### 4.4.查询roll购买状态
##### ___`wallet_info`___
##### 购买前的状态：  
<img width="240" alt="スクリーンショット 2021-07-18 20 57 24" src="https://user-images.githubusercontent.com/86814869/126066399-df5659bc-7572-4349-b306-6baf8e5b89bc.png">  

##### 购买进行中的状态：  
<img width="225" alt="スクリーンショット 2021-07-18 20 57 32" src="https://user-images.githubusercontent.com/86814869/126066411-bf1e7de3-e26b-4ed9-ac39-aef0df401ac4.png">  

##### 购买完成的状态：  
<img width="199" alt="スクリーンショット 2021-07-18 20 57 47" src="https://user-images.githubusercontent.com/86814869/126066424-3e1fe8c5-c521-49f6-a053-5830e870e907.png">  

##### 4.5.绑定钱包到massa节点以便进行质押操作(需要用到钱包私钥)  
##### ___`register_staking_keys <your_private_key>`___  
##### 4.6.查询roll的质押状态(大概10分钟左右)  
##### ___`wallet_info`___  
##### 质押完成的状态(active表示质押成功，系统开始随机选取质押节点进行区块创建，每创建一个区块奖励1MAS)：    
<img width="196" alt="スクリーンショット 2021-07-18 21 15 57" src="https://user-images.githubusercontent.com/86814869/126066657-db065711-cdd9-4148-a184-5361431ff41e.png">  

##### 4.7.赎回(卖出)roll（每个roll价值500个币,fee可填0,卖出完成大概1分钟左右可查询）  
##### ___`sell_rolls <wallet_address> <roll count> <fee>`___
##### 4.8.查询钱包状态  
##### ___`wallet_info`___

##### 5.输入选项5重启massa节点

#### ■ 注意事项
##### 1：此脚本仅支持Ubuntu系统和CentOS系统
##### 2：运行脚本安装Docker并下载TopMininG专供镜像进行节点部署（TopMininG专供镜像为官方编译的纯净打包版无任何修改可放心使用） 
##### 3：如因系统防火墙或云服务防火墙原因无法用次脚本下载安装Docker，请自行咨询服务商了解相应的Docker安装方法并手动安装Docker
##### 4：非TopMininG专供镜像部署的节点运行此脚本无效（TopMininG专供镜像为官方编译的纯净打包版无任何修改可放心使用） 
##### 5：Ubuntu系统需先执行sudo apt update 确保系统软件依赖包为最新
##### 6：Centos系统需先执行sudo yum update 确保系统软件依赖包为最新


#### ■ 常用链接：  
##### 1.massa官网：https://massa.net/
##### 2.massa区块浏览器：https://test.massa.net/#explorer
##### 3.massa官方水龙头：暂未公布细节(Discord领取测试币)
##### 4.massa官方Gitlab教程：https://gitlab.com/massalabs/massa/-/tree/dev
##### 5.massa官方文档：暂未公布细节
##### 6.massa路线图（Milestone）：暂未公布细节
##### 7.massa测试网奖励说明：https://massalabs.medium.com/massa-testnet-is-live-ed10a2a87272
##### 8.massa官方电报群：https://t.me/massanetwork
##### 9.massa官方Discord群：https://discord.com/invite/TnsJQzXkRN


