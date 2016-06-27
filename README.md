# FeedlySlackBot
Post unread article to slack by google apps script.

## Preparation for "google apps script"

1. Create empty google apps script project.

2. Rename XXXXXX.gs -> main.gs.

3. Get project key.

## Environment

Preparing the `.env` file with the following key-value.

|key|describe|
|:--|:-------|
|GAS_PROJECT_KEY|Project key at Google Apps Script|
|USER_NAME|User name to post|
|ICON_URL|Icon URL to post|
|SLACK_URL|Slack URL to post|

## Usage

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
