## Nativeアプリの実装

cordova pluginを使用してNativeアプリを作成します。

### 実機でNativeアプリをデバッグ実行する

Ionic DevAppを使用して実機でNativeアプリをデバッグ実行する  
（※参考：https://ionicframework.com/docs/appflow/devapp）
 
以下コマンドでデバッグ実行するプラットフォームを指定する

```
$ ionic cordova prepare ios
```
or
```
$ ionic cordova prepare android
```

以下コマンドでNativeアプリをデバッグ実行する

```
$ ionic serve --devapp
```

※1) デバッグ端末へのIonic DevApp（[AppStore](https://apps.apple.com/us/app/ionic-devapp/id1233447133) / [GooglePlay](https://play.google.com/store/apps/details?id=io.ionic.devapp)）の事前インストールが必要  
※2) Windows10では「Windows Defenderファイアウォール」の「受信の規則」に規則（ポート例：8100）の追加が必要  

+ 作業断面

対象ブランチ: `native/1` 

https://github.com/orinbou/ionic-hands-on-app/tree/native/1

### アイコン＆スプラッシュ画面を追加する

以下コマンドで必要なモジュールを事前インストールする

```
$ npm i -g cordova-res
```

以下コマンドでアイコン＆スプラッシュの画像を自動生成する

```
$ ionic cordova resources ios
```
or
```
$ ionic cordova resources android
```

### CircleCIでビルドできるようにする

以下のとおりNativeアプリのビルド設定ファイルを追加する。（※現在はAndroidアプリのみ対象とする）

* [編集内容はこちら](https://github.com/orinbou/ionic-hands-on-app/blob/native/circleci/.circleci/config.yml)

+ 作業断面

対象ブランチ: `native/circleci` 

https://github.com/orinbou/ionic-hands-on-app/tree/native/circleci

ここまでのソースコードの変更内容の全行は下記のとおり。

* [編集内容はこちら](https://github.com/orinbou/ionic-hands-on-app/compare/native/1...native/circleci)

### ビルドしたNativeアプリを実機で実行する

ビルドしたNativeアプリをdeploygateの下記URLからインストールする。

https://deploygate.com/users/orinbou/apps/jp.orinbou.ionic.hands.on.app

※事前にAndroidの開発者モードをONにして、提供元不明のアプリをインストールを許可しておく
