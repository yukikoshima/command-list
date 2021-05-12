### ファイル形式を変更、または移動

```
mv <ファイル名><ファイル名>
```

### 検索

```
find -name <検索したいファイル名>
```

### プロセス検索

```
lsof -i:8080
```

### 全てのプロセスを終了

```
killall
```

### シェルバージョン確認

```
/bin/<シェル名> --version
```

### インストールできるシェルの ver

```
brew info <シェル名>
```

### インストールされてるシェルとパスの確認

```
cat /etc/shells
```

### コマンド検索パスの確認方法

```
echo $PATH
```

### ログインシェル確認

```
echo $SHELL
```

### 現在、使用しているシェル

```
echo $0
```

### シェルの変更

```
chsh -s <変更したいシェル>
```

### /etc/shells にパスを追加

```
sudo sh -c "echo '/usr/local/bin/zsh' >> /etc/shells"
```

### httpd 起動

```
systemctl start httpd
```

### httpd 停止

```
systemctl stop httpd
```

### httpd ステータス確認

```
systemctl status httpd
```

### ファイアウォール起動

```
systemctl start firewalld
```

### ファイアウォール停止

```
systemctl stop firewalld
```

### ファイアウォールステータス確認

```
systemctl status firewalld
```

### ファイアウォールが動いているか確認

```
firewall-cmd —state
```

### ファイアウォールに http サービス追加

```
firewall-cmd --permanent --add-service=http
"--permanent"を付けるとサービスを再起動した場合にもこの設定を維持する
```

### ファイアウォール設定の更新

```
firewall-cmd —reload
```

### ファイアウォール設定を確認

```
firewall-cmd —list-all
```

### port3000 を開ける

```
firewall-cmd --permanent --add-port=3000/tcp
```

### http サービスの追加

```
firewall-cmd --permanent --add-service=http
```
