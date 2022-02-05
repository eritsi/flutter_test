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

### friendlychat
1. 左側シェルをwebディレクトリへ。  
2. 以下左側シェルで実行  
> npm install  
> npm run start  
3. `web/src/firebase-config.js` を編集  
削除 : `const config {}`  
追加 : My web app's Firebase configuration (Firebaseよりコピー)  
この時、 `getFirebaseConfig()` を残しつつ、 `config -> firebaseConfig` へ修正  
4. (必要に応じ) `web/firebase.json` を編集  
`"hosting"` に `"site"` 情報を追加  
> firebase deploy --only hosting:<サイト名>

## main.dartの例
widget_intro_examples以下  
https://flutter.dev/docs/development/ui/widgets-intro
