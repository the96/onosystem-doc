# githubの使い方
1. リポジトリをclone  
```
git clone URL
```

document  
> https://github.com/the96/onosystem-doc  
> git@github.com:the96/onosystem-doc  

serverside  
> https://github.com/the96/onosystem-server  
> git@github.com:the96/onosystem-server

android  
> https://github.com/the96/onosystem-android  
> git@github.com:the96/onosystem-android

2. branchを切る  
```
git checkout -b BRANCH_NAME
```
現在のbranchを確認する場合は
```
git branch
```

3. 作業内容をcommit & push  
```
git add FILE_PATH
git commit -m "COMMIT_MESSAGE"
git push origin BRANCH_NAME
```
変更したファイルがstaging(added)されているか確認する場合は
```
git status
```

4. pull requestを出す  
githubの該当リポジトリにアクセスし、pull requestを出す  
pull requestは確認が必要な変更の適用の場合のみ、pull requestを出す  
pull requestが必要ない場合はmaster branchにpushしてよい  

## githubにSSHで接続する方法
1. 秘密鍵と公開鍵を生成する
```
$ cd ~/.ssh
$ ssh-keygen -t rsa
```

2. githubに公開鍵をアップロード
```
github > Settings > SSH and GPG keys
```

### bash on ubuntu on windowsなどを利用している場合
Cドライブは`/mnt/c/`以下にある  
Windows側からUbuntuのデータにアクセスするのは難しい(複雑なので弄らないほうがよい)ので、公開鍵にWindowsからアクセスするときは、`/mnt/c/Users/USER/Documents`などにコピーすると良い。


### 関係リンク

* [sshでgithubに接続する方法](https://qiita.com/shizuma/items/2b2f873a0034839e47ce)

* [gitのremote urlを変更する](https://qiita.com/minoringo/items/917e325892733e0d606e)

* [gitブランチ関連コマンド](https://qiita.com/ayakix/items/55dc4a324a49ff200c2d)