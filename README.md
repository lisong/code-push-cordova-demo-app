# code-push-cordova-demo-app

# base on

fork from https://github.com/Microsoft/cordova-plugin-code-push examples

# iOS eg.

```shell
$ cd /path/to/code-push-cordova-demo-app
$ cordova prepare
$ cordova run ios
```

# android eg.

```shell
$ cd /path/to/code-push-cordova-demo-app
$ cordova prepare
$ cordova run android
```

# codepush 热更新

```shell
$ code-push login http://api.code-push.com:8080 #登录code-push-server
$ code-push app add CodePushCordovaDemo-ios  #iOS版
$ code-push app add CodePushCordovaDemo-android #android版
$ cd /path/to/code-push-cordova-demo-app
$ cordova prepare
$ code-push release-cordova CodePushCordovaDemo-ios ios -d Production #发布到code-push-server ios
$ code-push release-cordova CodePushCordovaDemo-android android -d Production #发布code-push-server android
```
