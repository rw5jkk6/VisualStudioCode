## VSCodeの説明
- taskやlauch、ユーザスニペットなどの設定の保存は各フォルダの隠しファイル(.vscode)にある

## ショートキー
|キー (win)|機能|
|:--|:-:|
|F1 または Ctrl+Shift+p|コマンドパレットの表示|
|opt(Alt)+shift+F|コードのフォーマット|
|F12|定義へ移動|
|cmd(Ctrl)+1\|2\|3|タブの移動|
|opt(Alt)+上下矢印|上下にコードを移動|
|shift+opt(Alt)+上下矢印|上下にコードをコピー|
|cmd+x|行のコピー、または削除|

## 機能
- ユーザースニペット
- task
  - .vscodeにある,task.jsonがない場合でないと、\[テンプレートからtask.jsonを生成]がでてこない 
  - コマンドパレットから\[タスクの構成]、テンプレートからtask.jsonを生成、others
  - tasks.jsonを書き直す
      ```json
      {
    "version": "2.0.0",
    "tasks": [
        {
            "label": "go run",
            "type": "shell",
            "command": "go",
            "args": [
                "run",
                "test.go"
            ],
            "problemMatcher": [],
            "group": {
                "kind": "build",
                "isDefault": true
            }
         }
      ]
    }
      ```
  - shift + command + b (初めての場合)
  - ビルドタスクを構成する。作ったのを選択する  (初めての場合)
  - shift + command + b で実行できる
- デバッガ

