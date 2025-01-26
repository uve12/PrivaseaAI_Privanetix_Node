# PrivaseaAI_Privanetix_Node

Technology that attests your human liveness to protect your digital presence from bots and AI impersonations.

**Raised : $15M**

---

# Join Crypto Console Community

Join TG : [Crypto Console Telegram](https://t.me/cryptoconsol) 

Follow X : [Crypto Console Twitter](https://www.x.com/cryptoconsol) 

Subscribe : [Crypto Console Youtube](https://www.youtube.com/@cryptoconsole)

---

## Hardware requirements:

| **Hardware** | **Minimum Requirement** | **Reccomended** |
|--------------|-------------------------|-----------------|
| **CPU**      | 4 Cores                 | 16 cores        |
| **RAM**      | 4 GB                    | 8 GB 	         |
| **Disk**     | 100  GB  SSD            | 100 GB SSD	     |

---

# VPS Options

💻 Contabo VPS Deals 🚀 Buy with Credit Card/Paypal/Crypto Credit card : 

Get powerful VPS solutions with these direct links:  


| **VPS** | **Direct Link**                      | **Specs**                                                                                              |
|---------|--------------------------------------|--------------------------------------------------------------------------------------------------------|
| VPS 1   | [Contabo VPS 1](https://www.jdoqocy.com/click-101278318-15692486) | 4 vCPU Cores, 4 GB RAM, 100 GB NVMe or 400 GB SSD     |
| VPS 2   | [Contabo VPS 2](https://www.anrdoezrs.net/click-101278318-13796472) | 6 vCPU Cores, 16 GB RAM, 200 GB NVMe or 400 GB SSD  |
| VPS 3   | [Contabo VPS 3](https://www.dpbolvw.net/click-101278318-13796474) | 8 vCPU Cores, 24 GB RAM, 300 GB NVMe or 1.2 TB SSD    |
| VPS 4   | [Contabo VPS 4](https://www.anrdoezrs.net/click-101278318-13796476) | 12 vCPU Cores, 48 GB RAM, 400 GB NVMe or 1.6 TB SSD |


💡 **Get started with the perfect VPS for your needs!** 🚀

---

### Testnet

Download ImHuman App

IOS : https://apps.apple.com/us/app/imhuman/id6482989056

Andriod : https://play.google.com/store/apps/details?id=com.app.imhuman

1. Create an account
- ref code : y98NrJs
2. Scan your biometric data
3. Your unique NFT is minted
4. Verify your facial vectors(Testify your liveness)
5. Copy ARB address from app and deposit around 0.002 ETH
6. Mint Facial vector data on ARB chain( 0.00167 Eth required)
7. Complete social tasks and earn stars.

### Update and Upgrade VPS

```
sudo apt update && sudo apt upgrade
sudo apt-get install ca-certificates curl
```

### Install Docker:

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg  
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null  
sudo apt-get update  
sudo apt-get install -y docker-ce docker-ce-cli containerd.io  
docker --version  
```
### Install Docker-Compose:

```
VER=$(curl -s https://api.github.com/repos/docker/compose/releases/latest | grep tag_name | cut -d '"' -f 4)  
sudo curl -L "https://github.com/docker/compose/releases/download/$VER/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose  
sudo chmod +x /usr/local/bin/docker-compose  
docker-compose --version  
```

### Docker Permission to User

```
sudo groupadd docker  
sudo usermod -aG docker $USER  
newgrp docker
```

### Pull Privasea docker Image

```
docker pull privasea/acceleration-node-beta:latest
```


### Create the program running directory and navigate to it:

```
mkdir -p  /privasea/config && cd  /privasea
```

### Create a new keystore file 

```
docker run -it -v "/privasea/config:/app/config" privasea/acceleration-node-beta:latest ./node-calc new_keystore
```

Note: The program will prompt you to enter a password, please remember this password for future use. The generated keystore file will have a corresponding node address, please save this address, it will be used in the dashboard configuration


**Example:**
```
Enter password for a new key:      # Enter wallet password  
Enter password again to verify:   # Re-enter the password for confirmation  
After successful creation of the wallet, the program will display information similar to the following:
```

**Sample:**
```
node address: 0xf07c3eF23ae7BEb8CD8bA5fF546E35Fd4b332B34
# This is the node address you generated, used for linking in the dashboard 
node filename: keystore:///app/config/UTC--2025-01-06T06-11-07.485797065Z--f07c3ef23ae7beb8cd8ba5ff546e35fd4b332b34

Instructions: 0xf07c3eF23ae7BEb8CD8bA5fF546E35Fd4b332B34 is an example and may differ in your case.
```

### Change to config directory 

```
cd /privasea/config && ls
```
### Rename the keystore file 

```
mv ./UTC--*  ./wallet_keystore 
```

### Link node address to reward address

- Visit : https://deepsea-beta.privasea.ai/privanetixNode

- Setup commission between 1 to 3 %


### Start the node

```
cd .. 
docker run  -d   -v "/privasea/config:/app/config" -e KEYSTORE_PASSWORD=123456 privasea/acceleration-node-beta:latest
```

### Check Node Health

```
docker logs -f 
```

---

Follow : https://x.com/cryptoconsol
