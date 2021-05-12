# git コマンド

**注意事項**
markdown 方式で記述すること

**お願い**
ここにないコマンドがあったら随時記述してってください

git をわかりやすく説明してくれてる動画:[クリック!!!
](https://www.youtube.com/watch?v=i1L3A0SLDyg)

### add

```
git add <ファイル名>
```

### add を全て取り消す

```
git reset HEAD
```

### commit ※-a で全て変更。-m でコメント　-am でも大丈夫。

```
git commit -a -m “コメント”
```

### リモートリポジトリに push

```
git push <push先のbrunch><pushするbranch>
```

### リモートリポジトリから最新情報を持ってくる。ただし pull みたいにファイルは更新されない。

```
git fetch
```

### 特定のコミットを取り消す

```
git revert <id 番号>
```

### ブランチ作成

```
git branch <ブランチ名>
```

### 今いるブランチを確認 (-a をつけることでリモートブランチもみれる)

```
git branch -a
```

### すでにある branch 名を変更する場合

```
git branch -M <oldbranch> <newbranch>
```

### ブランチ作成 and ブランチ切り替え

```
git checkout -b <ブランチ名>
```

### ブランチ変更

```
git checkout <ブランチ名>
```

### ブランチ削除

```
git branch -d <ブランチ名>
```

### マージ

```
git merge <ブランチ名>
```

### エイリアス

```
git config --global alias.<変更後><変更前>
```

### commit 履歴

```
git reflag
```

### 以前の commit 状態に戻す

```
git reset --hard <コミット ID>
```

### リモートブランチをローカルに持ってくるとき

```
1. git branch -a
2. git fetch —prune
3. git branch <ブランチ名> <origin/ブランチ名>
```

### リポジトリ内の特定のブランチを pull したい

```
git pull origin pull <したいリモートブランチ名:ローカルブランチ名>
```

### リモート先のブランチを消す

```
git push origin <:branchName>
```

### git 管理ファイルを検索

```
!git ls-files | grep -i
```

### Git でローカルの変更を元に戻す

```
git checkout <ファイル名>
git checkout . ※ドットは全部
```

### ローカルで作成したリポジトリをリモートにプッシュする

```
cd <フォルダ名>
git init
git remote add origin https://gitlab.com/yuki30088967/commandlist.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

### 拡張子を変更

```
git mv <変更前> <変更後>
```
