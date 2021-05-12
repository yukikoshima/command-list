# npm コマンド

**注意事項**  
markdown 方式で記述すること

**お願い**  
ここにないコマンドがあったら随時記述してってください

### node インストール手順(mac)

```
brew install nodebrew

echo 'export PATH=$HOME/.nodebrew/current/bin:$PATH' >> ~/.zshrc

nodebrew setup

nodebrew install-binary stable
```

### package.json 作成

```
npm init -yes
```

### インストールしたパッケージ確認(-g:グローバル)

```
npm -g list --depth=0
```

### 実行中のプロセス検索

```
ps aux | grep node
```

### プロセス切断

```
sudo kill -9 <id>
```

### グローバルの node_module ディレクトリを探す

```
npm root -g
```

### express generator インストール

```
npm install express-generator
```

### express generator

```
express -e アプリケーション名
```
