## レポートを修正する

1. slackのbotとして動作する
1. botは@replyでコマンドとレポートIDとレポートを受け付ける
1. 受け付けるコマンドは`post #<レポートID> <レポート>`
1. botは受け付けたレポートIDに紐つくレポートを、誰から・どんな内容での２つに分解する
	- 代替コース：受け付けたレポートIDに紐つくレポートが存在しない場合は、`404 Not Found`を返して終わる。
1. 履歴は保存しない
1. 改善状態を変更しない

```
@incident #0104503 Bプロジェクトでパスワードの長さが英数４桁だった。少なくとも英数記号以上にしなければ暗号強度が低すぎて辞書攻撃で破られてしまう。
```