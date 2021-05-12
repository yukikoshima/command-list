### mysql 起動

```
mysql.server start
```

### mysql 終了

```
mysql.server stop
```

### mysql 状態確認

```
mysql.server status
```

### mysql ログイン

```
mysql -u <ユーザー名> -p
(データベースを指名する時は)
mysql -u <ユーザー名> -D <データベース名> -p
```

### mysql パスワードなしでログイン

```
mysql.server start —skip-grant-tables
```

### mysql バージョン確認

```
mysql —version
```

### パスワード設定

```
set password for root@localhost=password(‘’hogehoge);
```

### データベース一覧

```
show databases
```

### データベース作成

```
create database <データベース名>
```

### データベース削除

```
drop database <データベース名>
```

### 使用するデータベースを選択

```
use <データベース名>
```

### テーブル名を一覧

```
show tables
```

### テーブルの構造を表示

```
desc <テーブル名>
```

### SQL モードを確認する

```
show variables like ‘sql_mode’
```

### ターミナルモードの文字コーディングを変更<utf8 だったら>

```
set names <utf8>
```

### 文字コードデフォルト参照

```
show variables like ‘chara%’
```

### ユーザー名を確認

```
select host,user from mysql.user
```

### ユーザー名を変更

```
rename user <old_user@ホスト名> to <new_user@ホスト名>
```

### パスワード変更

```
ALTER USER 'root'@'localhost' IDENTIFIED BY 'MyNewPass';
```

### ホスト名を確認

```
show variables like ‘hostname’
```
