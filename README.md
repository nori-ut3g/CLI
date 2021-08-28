#CLI

#Description
疑似的なコマンドラインです。
以下のコマンドを実行できるようにしました。
上下キーで過去のコマンドを
```angular2html
ls [|filepath] [-option]
pwd []
touch [filePath]
tree [|filepath]
mkdir [filepath]
cd [filepath]
rm [filepath] [-option]
adduser [username]
login [username]
logout
passwd [|username]
chmod [permissionSetting] [filepath]
chown [username|:group|username:group] [filepath]
mv [filepath] [filepath]
cp [filepath] [filepath]
```

##各コマンドの特徴
#ls
カレントディレクトリ内にあるフォルダやファイルの一覧を表示します。
オプション　-l
フォルダやファイルのPermission、Group、作成日時などの詳細情報を表示します。
オプション -a
.から始まる隠しファイルも表示します。

#tree
現在のディレクトリから隠しファイルを含めたすべてのフォルダ、ファイルをツリー表示します。

#adduser
ユーザーを追加します。
同時にユーザーのホームディレクトリが作成されます。

#login
指定のユーザーアカウントにログインします。
パスワードが設定されている場合は、パスワードを設定します。

#logout
rootユーザーに戻ります。

#passwd
自分のアカウントにログインパスワードを設定します。
rootユーザー時は、ユーザーを指定することもできます。
ハッシュ値でパスワードを保存しています。

#chmod
ファイルやディレクトリの権限を変更します。
今回の