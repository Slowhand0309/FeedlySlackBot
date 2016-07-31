# FeedlySlackBot
Post unread article to slack by google apps script.

未読の記事をSlackにGoogle Apps Scriptを使ってポストします。

## Preparation for "google apps script"

Google Apps Script側の準備

1. Create empty google apps script project.

空のGoogle Apps Scriptプロジェクトを作成します。

![img1](https://raw.githubusercontent.com/Slowhand0309/FeedlySlackBot/master/doc/img1.png)

2. Rename XXXXXX.gs -> main.gs.

ファイル名をコード.gsからmain.gsに変更します。

![img2](https://raw.githubusercontent.com/Slowhand0309/FeedlySlackBot/master/doc/img2.png)

![img3](https://raw.githubusercontent.com/Slowhand0309/FeedlySlackBot/master/doc/img3.png)

3. Get project key.

プロジェクトキーを取得します。

![img4](https://raw.githubusercontent.com/Slowhand0309/FeedlySlackBot/master/doc/img4.png)

![img5](https://raw.githubusercontent.com/Slowhand0309/FeedlySlackBot/master/doc/img5.png)


## Environment

環境設定

Preparing the `.env` file with the following key-value.

次に以下のKey-Valueでプロジェクト直下に`.env`ファイルを作成します。

|key|describe|説明|
|:--|:-------|:--|
|GAS_PROJECT_KEY|Project key at Google Apps Script|Google Apps Scriptのプロジェクトキー|
|ACCESS_TOKEN|Feedly access token|Feedlyのアクセストークン|
|POST_CHANNEL|Post slack channel|ポストするSlackのチャンネル|
|USER_NAME|User name to post|ポストするBot名|
|ICON_URL|Icon URL to post|ポストするBotのアイコンURL|
|SLACK_URL|Slack URL to post|ポストするSlackのURL|
|MAX_FEED_POST|Max feed post|ポストするfeed毎の最大件数|

## Usage

使用方法

Synchronized with the project of Google apps script.<br>
Google apps scriptプロジェクトと同期します。

```sh
$ grunt init
```

Generate script file `main.js` by template.<br>
テンプレートから`main.js`を作成します。

```sh
$ grunt
```

Deploy script file.<br>
`main.js`をアップロードします。

```sh
$ grunt upload
```

## Licence

MIT

## Author

[slowhand0309](https://github.com/Slowhand0309)
