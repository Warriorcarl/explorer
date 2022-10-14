<div align="center">

![Ping Wallet](./public/logo.svg)

# Set up Explorer for your cosmos chains

## 1. Update packages
```
sudo apt update && sudo apt upgrade -y
```

## 2. Install nginx
```
sudo apt install nginx -y
```

## 3. Install nodejs
```
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt-get install -y nodejs
```

### 4. Install yarn
```
curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | gpg --dearmor | sudo tee /usr/share/keyrings/yarnkey.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/yarnkey.gpg] https://dl.yarnpkg.com/debian stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update && sudo apt-get install yarn
```

## 3. Install binaries
```
cd ~
git clone https://github.com/Warriorcarl/explorer.git
cd explorer
```

## 6. Build Explorer
```
yarn && yarn build
cp -r $HOME/explorer/dist/* /var/www/html
sudo systemctl restart nginx
```

## Donation

Your donation will help us make better products. Thanks in advance.

 - Address for ERC20: USDC, USDT, ETH
```
0x88BFec573Dd3E4b7d2E6BfD4D0D6B11F843F8aa1
```

 - You can donate any token in the Cosmos ecosystem: [here](https://ping.pub/coffee)

> If you are an individual please do not donate more than $10, a cup of coffee means a lot to us.

#### Donations from project

- Point Network: 1000USDC and $1000 worth of POINT
- Bitsong: 50k BTSG
- IRISnet: 100k IRIS


## Contributors
Developers: @liangping @dingyiming

