## アプリケーションの作成

Ionic CLIでアプリケーションを作成・起動します。

* 作業ブランチINDEX  
https://github.com/orinbou/ionic-hands-on-app/tree/startup/1
https://github.com/orinbou/ionic-hands-on-app/tree/startup/2
https://github.com/orinbou/ionic-hands-on-app/tree/startup/3

### ionic cli でアプリケーションを作成する

以下コマンドでアプリケーションを作成する

```
$ ionic start ionic-hands-on-app blank --type=angular
```

以下のようにアプリケーションが作成される

```
√ Preparing directory .\ionic-hands-on-app - done!
√ Downloading and extracting blank starter - done!

Installing dependencies may take several minutes.

  ──────────────────────────────────────────────────────────────

        Ionic Appflow, the mobile DevOps solution by Ionic

           Continuously build, deploy, and ship apps
        Focus on building apps while we automate the rest

        Learn more: https://ion.link/appflow

  ──────────────────────────────────────────────────────────────
> npm.cmd i

（....中略....）

[INFO] Next Steps:

       - Go to your newly created project: cd .\ionic-hands-on-app
       - Run ionic serve within the app directory to see your app
       - Build features and components: https://ion.link/scaffolding-docs
       - Get Ionic DevApp for easy device testing: https://ion.link/devapp
```

### アプリケーションを起動する

下記のコマンドを実行する。

```
$ cd ionic-hands-on-app
$ ionic serve
```

アプリケーションが起動してWebブラウザに表示される

※Webブラウザに自動表示されない場合は下記URLを開いて確認すること！

http://localhost:8100 へブラウザで接続すると、

サンプルアプリケーションが表示される

+ 作業断面

対象ブランチ: `startup/1` 

https://github.com/orinbou/ionic-hands-on-app/tree/startup/1

### サンプルアプリの編集

以下のとおりソースコードを編集する。

* [編集内容はこちら](https://github.com/orinbou/ionic-hands-on-app/compare/startup/1...startup/2)

編集して、保存すると、画面に即座に反映される

※タイトルバーの色が変わる（白→青）

+ 作業断面

対象ブランチ: `startup/2` 

https://github.com/orinbou/ionic-hands-on-app/tree/startup/2

### プラットフォーム毎の表示を確認する

下記のコマンドを実行する。

```
$ ionic serve --lab
```

アプリケーションが起動してWebブラウザに表示される

※Webブラウザに自動表示されない場合は下記URLを開いて確認すること！

http://localhost:8200 へブラウザで接続すると、

サンプルアプリケーションが表示される

+ 作業断面

対象ブランチ: `startup/3` 

https://github.com/orinbou/ionic-hands-on-app/tree/startup/3
