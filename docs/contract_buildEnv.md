# How to build develop environment for contract

## 1. Get Private Key of your metamask

コントラクトをネットワークにデプロイするためにはガス代がかかります。そのガス代は自分のウォレットもしくはチームのウォレットから支払う必要があります。  
デプロイスクリプトとウォレットを接続するために、メタマスクの Private Key が必要です。この Private Key は他の誰かに渡すことがないようにしてください。そして、.env ファイルにキーを保存して github には絶対に上げないでください。

For deploying contract to network, deployer need gas fee for deploy.

### 1.1 アカウントの詳細画面をひらく

<img src="./documentImages/privatekey_1.png" width="300px" />

### 1.2 秘密鍵のエクスポートを押下

<img src="./documentImages/privatekey_2.png" width="300px" />

### 1.3 　ウォレットのパスワードを入力

<img src="./documentImages/privatekey_3.png" width="300px" />

### 1.4 秘密鍵をコピー

<img src="./documentImages/privatekey_4.png" width="300px" />

### .env ファイルに秘密鍵をセット

.env.example をもとに.env をつくって、LOCAL_PRIVATE_KEY に 1.4 でコピーした秘密鍵をセット。テストネット、メインネットにデプロイなどをする場合は、PRIVATE_KEY にもセット。
