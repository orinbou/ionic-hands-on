## Nativeアプリの実装2

cordova pluginを使用してNative機能（カメラ）と連携できるようにします。
（※参考：https://ionicframework.com/jp/docs/angular/your-first-app/ios-android-camera）

* 作業ブランチINDEX  
https://github.com/orinbou/ionic-hands-on-app/tree/camera/1
https://github.com/orinbou/ionic-hands-on-app/tree/camera/2

### CLI を介してカメラの依存関係を追加

以下コマンドでCamera APIを使用して端末でカメラをで使用できるようにする

```
$ npm install @ionic-native/camera
$ ionic cordova plugin add cordova-plugin-camera
```

+ 作業断面

対象ブランチ: `camera/1` 

https://github.com/orinbou/ionic-hands-on-app/tree/camera/1

### カメラ撮影機能を実装する

以下のとおりソースコードを編集する。

* [編集内容はこちら](https://github.com/orinbou/ionic-hands-on-app/compare/camera/1...camera/2)

編集して、保存すると、画面に即座に反映される

※画面にカメラボタンが表示されるが、Webシミュレータでは実行できないため実機で確認する

+ 作業断面

対象ブランチ: `camera/2` 

https://github.com/orinbou/ionic-hands-on-app/tree/camera/2
