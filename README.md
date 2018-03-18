# Intermodal
Shell script to install a [Intermodal Coin asternode](http://intermodalcoin.online/) on a Linux server running Ubuntu 16.04. Use it on your own risk.
***

## Installation
```
wget -q https://raw.githubusercontent.com/zoldur/Intermodal/master/intermodal_install.sh  
bash intermodal_install.sh
```
***

## Desktop wallet setup  

After the MN is up and running, you need to configure the desktop wallet accordingly. Here are the steps:  
1. Open the Intermodal Desktop Wallet.  
2. Go to RECEIVE and create a New Address: **MN1**  
3. Send **5000** IMC to **MN1**.  
4. Wait for 15 confirmations.  
5. Go to **Help -> "Debug Window - Console"**  
6. Type the following command: **masternode outputs**  
7. Go to **Masternodes** tab  
8. Click **Create** and fill the details:  
* Alias: **MN1**  
* Address: **VPS_IP:PORT**  
* Privkey: **Masternode Private Key**  
* TxHash: **First value from Step 6**  
* Output index:  **Second value from Step 6**  
* Reward address: leave blank  
* Reward %: leave blank 
9. Click **OK** to add the masternode  
10. Click **Start All**  
***

## Usage:
```
Intermodald masternode status #This will show whether your MN is active or not. If status is 9, you are good to go.
Intermodald getinfo
```
Also, if you want to check/start/stop **Intermodal**, run one of the following commands as **root**:

```
systemctl status Intermodal #To check if Intermodal service is running  
systemctl start Intermodal #To start Intermodal service  
systemctl stop Intermodal #To stop Intermodal service  
systemctl is-enabled Intermodal #To check if Intermodal service is enabled on boot  
```  
***

## Donations

Any donation is highly appreciated  

  
**BTC**: 3MQLEcHXVvxpmwbB811qiC1c6g21ZKa7Jh  
**ETH**: 0x26B9dDa0616FE0759273D651e77Fe7dd7751E01E  
**LTC**: LNZpK4rCd1JVSB3rGKTAnTkudV9So9zexB  
