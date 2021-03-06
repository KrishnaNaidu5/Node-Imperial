# How to mine WebDollar with Linux Terminal
Mine WebDollar with Linux Terminal

### 1. Automatic Install and Clone
```shell
git clone https://github.com/WebDollar/Node-WebDollar.git Node-WebDollar1 #Note: it is recommended to clone WebDollar repo in your home user folder, eg: /home/YOUR_USER/
cd Node-WebDollar1
bash install-miner.sh
```
### 2. Manual Install and Clone:
```shell
sudo apt-get update -y && sudo apt-get upgrade -y && sudo apt install -y linuxbrew-wrapper && sudo apt-get install -y build-essential && sudo apt-get install -y clang
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
source ~/.profile
nvm install 16
nvm use 16
nvm alias default 16
npm install -g node-gyp && npm install pm2 -g --unsafe-perm
git clone https://github.com/WebDollar/Node-WebDollar.git Node-WebDollar1 # Note: it is recommended to clone WebDollar repo in your home user folder, eg: /home/YOUR_USER/
cd Node-WebDollar1
npm install
```
### 3. Use argon2 CPP Optimization
```shell
bash build-argon2.sh
```
### 4. Run miner
```shell
npm run commands
```
### 5. Fastest way to mine
#### press ```10``` then hit Enter; paste POOL LINK then hit ENTER.

### 6. SOLO-MINING
#### Before starting SOLO-Mining you need to download the blockchain bootstrap!
#### Blockchain bootstrap locations and instructions can be found <a href="https://github.com/WebDollar/Node-WebDollar/blob/master/tutorials/blockchain-bootstrap-locations.md">HERE!</a>
----
### **Create a password for your WebDollar Wallet**
#### -> After you run ```npm run commands```, press ```6``` then press ```0``` (0 is your first address in your Wallet). Copy/paste a 12 word passphrase and press enter
#### -> Warning: make sure you backup your passphrase very well. If you loose it, your wallet is gone forever!
----
### **Save your Wallet to your storage**
#### -> Press ```5``` then press ```0``` (0 is your first address in your Wallet) then enter a location where it should be saved. 
   Example: ```/home/webd1/Node-WebDollar1/```
#### -> If you see the message, "Address Exported Successfully!" your address was saved.
----
### **How to update Miner instance**
#### -> Stop mining with ```ctrl + c``` (better stop it after you see the message *Saving Blockchain Starting from x y*) then run ```update.sh```
#### -> Start mining again with ```npm run commands``` and ```8```
----
### Blockchain Loading and Saving example ###
<img src="https://www.vpnromania.ro/webd/webdollar-saving-blockchain-img1.jpg" alt="Blockchain Loading Example" /></img>
----
### WebDollar Mining Example
<img src="https://www.vpnromania.ro/webd/webdollar-mining-img1.jpg" alt="WebDollar Mining Example" /></img>
