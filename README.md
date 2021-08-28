#CLI

#Description
疑似的なコマンドラインです。
以下のコマンドを実行できるようにしました。
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
passwd [|username]
chmod [permissionSetting] [filepath]
chown [username|:group|username:group] [filepath]
mv [filepath] [filepath]
cp [filepath] [filepath]
```

##Fe
よりリアルなコマンドラインを実現するためにファイル、ディレクトリのパーミッションを追加しました。
