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
