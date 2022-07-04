## 書き方と実行
- .vscodeにある,task.jsonがない場合でないと、\[テンプレートからtask.jsonを生成]がでてこない 
- コマンドパレットから\[タスクの構成]、テンプレートからtask.jsonを生成、others
- tasks.jsonを書き直す
- shift + command + b (初めての場合)
- ビルドタスクを構成する。作ったのを選択する  (初めての場合)
- shift + command + b で実行できる
## jsonのキーの意味
|キー|意味|
|:-:|:--|
|label|タスクの名前で実行時に見分けるもの名前|
|type|ほとんど shell|
|command|コマンド名　　例えば go, gcc, python3など|
|args|コマンドの後に続く引数、オプションやファイル名など|
