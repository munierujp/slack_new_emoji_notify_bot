[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

# slack_new_emoji_notify_bot
Slackの新規絵文字を通知するBOT

## プロパティ
|プロパティ|説明|例|
|---|---|---|
|`MESSAGE_TEMPLATE`|メッセージのテンプレート|`:{{name}}: ({{name}}) has added on {{added}}.`|
|`MESSAGE_TEMPLATE_ADDED_FORMAT`|メッセージのテンプレートの`added`のフォーマット|`YYYY[/]M[/]D H[:]mm[:]ss`|
|`MESSAGE_TEMPLATE_DATE_LANG`|メッセージのテンプレートの日付の言語|`ja`|
|`WEBHOOK_URL`|SlackのWebhook URL|`https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX`|

### MESSAGE_TEMPLATE
以下の変数を用いて、[Mustache.js](https://github.com/janl/mustache.js/)の記法で書けます。

|変数|説明|例|
|---|---|---|
|`name`|絵文字名|`picard_facepalm`|
|`url`|絵文字のURL|`https://my.slack.com/emoji/picard_facepalm/db8e287430eaa459.gif`|
|`added`|追加日持|`2013-02-21T21:41:56.000Z`|

### MESSAGE_TEMPLATE_DATE_LANG
以下の言語を指定できます。  
指定しなかった場合や、これ以外の値を指定した場合は英語になります。

|値|説明|
|---|---|
|`ja`|日本語|

## ライブラリ
* Moment  
`MHMchiX6c1bwSqGM1PZiW_PxhMjh3Sh48`
* Mustache  
`MoB1GsrPeNTPPX8SRqpw8QDVZgzu5bsVr`
