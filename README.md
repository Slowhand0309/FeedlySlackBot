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

|key|describe|
|:--|:-------|
|GAS_PROJECT_KEY|Project key at Google Apps Script|
|ACCESS_TOKEN|Feedly access token|
|POST_CHANNEL|Post slack channel|
|USER_NAME|User name to post|
|ICON_URL|Icon URL to post|
|SLACK_URL|Slack URL to post|

## Usage

使用方法

Synchronized with the project of Google apps script.

```sh
$ grunt init
```

Generate script file `main.js` by template.

```sh
$ grunt
```

Deploy script file.

```sh
$ grunt upload
```

## Licence

MIT

## Author

[slowhand0309](https://github.com/Slowhand0309)
