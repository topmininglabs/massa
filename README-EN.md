## Massa Testnet v0.1.0 Docker One-click deployment script（Ubuntu&CentOS）

#### ■ One-click script running method (copy and paste the entire line to execute).
  
##### ・Ubuntu：
##### ___`sudo apt update && sudo apt-get install wget curl`___
##### ・CentOS7：
##### ___`sudo yum update && sudo yum install wget curl`___
##### ・CentOS8：
##### ___`sudo yum update --nobest && sudo yum install wget curl`___
##### 
##### ___`wget https://github.com/topmininglabs/massa/raw/main/topmining_massa.sh.x && chmod +x ./topmining_massa.sh.x && sudo ./topmining_massa.sh.x`___
#####   

#### ■ Operation Guide：
<img width="383" alt="スクリーンショット 2021-07-19 0 57 38" src="https://user-images.githubusercontent.com/86814869/126073968-953966e5-e2a7-4d23-8fac-f7d0b8ec0644.png">

##### 1.Enter option 1 to install Docker
##### 2.Enter option 2 to download the TopMininG image exclusively for massa
##### 3.Enter option 3 to run the massa container node
##### 4 Enter option 4 to enter the node wallet interaction interface for wallet operations and pledge operations
##### 4.1.Create a new wallet (please keep the wallet address and private key)
##### ___`wallet_new_privkey`___
##### 4.2.Check wallet information (make sure you have enough test coins, you can get test coins through the official Discord at the bottom)
##### ___`wallet_info`___
##### 4.3.Buy roll (buy a roll need 500 coins, fee can fill in 0)
##### ___`buy_rolls <wallet_address> <roll count> <fee>`___
##### 4.4.Check roll purchase status
##### ___`wallet_info`___
##### Status before purchase：  
<img width="240" alt="スクリーンショット 2021-07-18 20 57 24" src="https://user-images.githubusercontent.com/86814869/126066399-df5659bc-7572-4349-b306-6baf8e5b89bc.png">  

##### Purchase in progress status：  
<img width="225" alt="スクリーンショット 2021-07-18 20 57 32" src="https://user-images.githubusercontent.com/86814869/126066411-bf1e7de3-e26b-4ed9-ac39-aef0df401ac4.png">  

##### Status of completed purchase：  
<img width="199" alt="スクリーンショット 2021-07-18 20 57 47" src="https://user-images.githubusercontent.com/86814869/126066424-3e1fe8c5-c521-49f6-a053-5830e870e907.png">  

##### 4.5.Bind the wallet to the massa node for pledge operations (requires the wallet private key)  
##### ___`register_staking_keys <your_private_key>`___  
##### 4.6.Check the status of roll's pledge (about 10 minutes)  
##### ___`wallet_info`___  
##### Pledge completion status (active means pledge is successful and the system starts randomly selecting pledge nodes for block creation, with 1MAS reward for each block created)：    
<img width="196" alt="スクリーンショット 2021-07-18 21 15 57" src="https://user-images.githubusercontent.com/86814869/126066657-db065711-cdd9-4148-a184-5361431ff41e.png">  

##### 4.7.Redemption (sell) roll (each roll is worth 500 coins, fee can be filled with 0, sell completion can be checked in about 1 minute)  
##### ___`sell_rolls <wallet_address> <roll count> <fee>`___
##### 4.8.Check Wallet Status  
##### ___`wallet_info`___

##### 5.Enter option 5 to restart the massa node
##### 6.Enter option 6 to update the massa node

#### ■ Caution
##### 1: This script only supports Ubuntu system and CentOS system
##### 2：Run the script to install Docker and download TopMininG exclusive image for node deployment (TopMininG exclusive image is the official compiled pure packaged version without any modification can be used without any worries) 
##### 3: If you can't download and install Docker by subscript due to system firewall or cloud service firewall, please consult your service provider to understand the corresponding Docker installation method and install Docker manually.
##### 4：Nodes that are not deployed with TopMininG exclusive mirror are not valid to run this script (TopMininG exclusive mirror is the official compiled pure packaged version without any modification can be used with confidence) 
##### 5：Ubuntu system need to execute sudo apt update first to ensure the system software dependency package is the latest
##### 6：Centos system need to execute sudo yum update first to ensure that the system software dependency package is the latest

#### ■ Useful Link：  
##### 1.Massa Official Website：https://massa.net/
##### 2.Massa Block Ecplorer ：https://test.massa.net/#explorer
##### 3.Massa Faucet：No details released yet(can get test coin via Discord)
##### 4.Massa Official Gitlab：https://gitlab.com/massalabs/massa/-/tree/dev
##### 5.Massa Official Tutorials：No details released yet
##### 6.Massa Milestone：No details released yet
##### 7.Massa Testnet：https://massalabs.medium.com/massa-testnet-is-live-ed10a2a87272
##### 8.Massa Official Telegram：https://t.me/massanetwork
##### 9.Massa Official Discord：https://discord.com/invite/TnsJQzXkRN


