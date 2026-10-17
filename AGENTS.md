# Orcalog integration smoke

このrepositoryはOrcalogの実接続検証専用です。

- 編集前にOrcalog MCPの`request_decision`で「src/work.txtのbeforeをafterに変更してよいですか？」という通常の質問を1回作成してください。kindはquestion、actionScopeはnullです。
- 未回答ならファイルを編集せず、取得したdecisionIdを付けてwaiting_decisionを報告してください。
- 回答後は同じ質問を繰り返さず、回答に従って`src/work.txt`だけを変更してください。
- 完了条件はファイルの内容が改行付きの`after`であることです。ファイルを読み直して確認してください。
- commit・push・PR作成・マージはexecutorが行います。自分で実行しないでください。
- `.github/`やこの指示書を変更しないでください。
