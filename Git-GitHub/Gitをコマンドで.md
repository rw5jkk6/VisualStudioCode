## Goのコードを書くにあたってGitをコマンドで使う
### 問題(基礎)
- Gitを初期化する
- masterブランチでファイルを作って、add関数を作って実行する。ステージングしてコミットする
- ブランチを作ってsub関数を作る。ステージングしてコミットする
- masterブランチからmergeする
- 使ったブランチを削除する

### 解答(基礎)
- Gitを初期化する
  - `git init`
- masterブランチでファイルを作って、add関数を作って実行する。ステージングしてコミットする
  - ファイルを作る。add関数を書いて実行して試す
  - `go mod init ファイル名` `go mod tidy`
  - `git add . `
  - `git commit -m "メッセージ"`
- ブランチを作ってsub関数を作る。ステージングしてコミットする
  - 初めにブランチを確認する `git branch`
  - ブランチを作成する `git branch ブランチ名`
  - ブランチに移動 `git checkout ブランチ名` 
  - sub関数を書いて実行する
  - `git add . `
  - `git commit -m "メッセージ"` 
- masterブランチからmergeする
  - masterブランチに戻る `git checkout master`
  - mergeする `git merge ブランチ名` 
- 使ったブランチを削除する
  - `git branch -d ブランチ名` 

### 問題(応用)
- testを書く
  - ライブラリのテストを書く。main.goがないので、テストを書かないと正確性が検証できない
  - GitHubActionsを使う 
