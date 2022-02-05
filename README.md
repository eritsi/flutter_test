# flutter_test
flutterの環境構築リポジトリ

## Codelabに合流するには
gitpodの右ターミナルで
 - startup_namer [Flutter]
 - friendlychat [javascript]
 - friendlyeats-flutter [Flutter] 
と回答し、それぞれ以下のCodelabに合流できる  
https://codelabs.developers.google.com/codelabs/first-flutter-app-pt1#2  
https://firebase.google.com/codelabs/firebase-web#2
https://codelabs.developers.google.com/codelabs/friendlyeats-flutter#2

## GitPodを使う際の注意
FirebaseのAuthentificationにおいて、承認済みドメインとしてlocalhostはデフォルトで入っているが、GitPodがホスティングしているプライベートドメインはlocalhostではない扱いになるのでアクセスできない。GitPodごとに承認済みドメインに登録すること。

### startup_namer  
1. Stateful, Stateless Widgetを学ぶ
2. pubspec.yaml への登録 `flutter pub add english_words` のコマンド  

## main.dartの例
widget_intro_examples以下  
https://flutter.dev/docs/development/ui/widgets-intro
