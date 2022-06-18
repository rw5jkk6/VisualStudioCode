## VSCodeの説明
- taskやlauch、ユーザスニペットなどの設定の保存は各フォルダの隠しファイル(.vscode)にある

## ショートキー


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
  - ctrl + command + b
  - ビルドタスクを構成する。作ったのを選択する
  - ctrl + command + b で実行できる
- デバッガ

