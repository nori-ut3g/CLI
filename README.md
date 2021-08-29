# CLI(Recursion Project6)

## 概要
疑似的なコマンドラインです。Recursionの課題の一環で下記コマンドを実装しました。コードはオリジナルです。

```angular2html
ls [|filepath] [-option]
pwd []
touch [filePath]
mkdir [filepath]
cd [filepath]
rm [filepath] [-option]
mv [filepath] [filepath]
cp [filepath] [filepath]
```

また、課題にはない下記コマンドも追加しました。

```angular2html
tree [|filepath]
adduser [username]
login [username]
logout
passwd [|username]
chmod [permissionSetting] [filepath]
chown [username|:group|username:group] [filepath]
```
Filepathは絶対パス、相対パスに対応し、~でログイン中のアカウントのHomeディレクトリを指定できます。

アカウントにパスワードを設定することもでき、パスワードはハッシュ値で保存しました。

ファイル、ディレクトリにPermissionが指定できるようにし、ほかのアカウントからのアクセスを制限することもできます。

### 各コマンドの特徴
#### ls
カレントディレクトリ内にあるフォルダやファイルの一覧を表示します。
オプション　-l
フォルダやファイルのPermission、Group、作成日時などの詳細情報を表示します。
オプション -a
.から始まる隠しファイルも表示します。

#### pwd

#### touch

#### mkdir

#### cd

#### rm

#### mv

#### cp

#### tree
現在のディレクトリから隠しファイルを含めたすべてのフォルダ、ファイルをツリー表示します。

#### adduser
ユーザーを追加します。
同時にユーザーのホームディレクトリが作成されます。

#### login
指定のユーザーアカウントにログインします。
パスワードが設定されている場合は、パスワードを設定します。

#### logout
rootユーザーに戻ります。

#### passwd
自分のアカウントにログインパスワードを設定します。
rootユーザー時は、ユーザーを指定することもできます。
ハッシュ値でパスワードを保存しています。

#### chmod
ファイルやディレクトリの権限を変更します。
今回の

#### chown