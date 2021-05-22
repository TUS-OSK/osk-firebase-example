# osk-firebase-example

Firebase の使い方に関する例と知見を得られます！

## プロジェクトの設定

https://firebase.google.com/docs/projects/learn-more?hl=ja

> **【先輩が教えてくれた知見メモ】**
>
> Web Apps 用の **apiKey** は公開しても大丈夫だが、**セキュリティルール**を設定しよう！
>
> - **apiKey** というのは、例えば FireStore を利用してデータ取得を叩いたりする時に使うような API キーです([apiKey に関して](https://firebase.google.com/docs/projects/api-keys?hl=ja))
> - **セキュリティルール** というのは、FireStore を利用するときに、アクセスしようとしているパス(叩こうとしているクエリ)に応じて read,write,delete の権限を設定できるものです([セキュリティルールに関して](https://firebase.google.com/docs/firestore/security/get-started?hl=ja))
> - **セキュリティルール** を使って、リクエストに乗っている、ユーザー毎に振り分けられる uid に対応する部分だけ権限を渡す、などが可能になります
>
> ただし、セキュリティルール以外にも権限をつける方法はあります
>
> - Google Cloud Platform のコンソールで[API とサービス>認証情報](https://console.cloud.google.com/apis/credentials?hl=ja)パネルから、各プロジェクトの Browser key をドメインや IP アドレスで制限できます
> - FireStore 自体の設定でも、同様にドメインなどから制限することができます

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
