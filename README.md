## VSCodeのバージョンの確認方法、更新
- バージョン情報(更新は下の書いてる近くにある)
  - (mac) メニューバーの`Code`の`バージョン情報`
  - (windows) `ヘルプ` `バージョン情報`  
- 更新でエラーできないのはvscodeがダウンロードフォルダ(ReadOnly)にあるので、アプリケーションフォルダに移動させる必要がある。メニューバーでFinder表示の時に移動を選択する。ダウンロードとアプリケーションの２つをopenしてvscodeアプリを移動させる 
## VSCodeの説明
- taskやlauch、ユーザスニペットなどの設定の保存は各フォルダの隠しファイル(.vscode)にある

## ショートキー
|キー (win)|機能|
|:--|:--|
|F1 または Ctrl+Shift+p|コマンドパレットの表示|
|opt(Alt)+shift+F|コードのフォーマット|
|F12|定義へ移動|
|cmd(Ctrl)+1\|2\|3|タブの移動|
|opt(Alt)+上下矢印|上下にコードを移動|
|shift+opt(Alt)+上下矢印|上下にコードをコピー|
|cmd+x|行のコピー、または削除|
|cmd + shift + b|タスクの実行|
|cmd + j　または ctrl + ` <br>(windows)Alt ＋ チルダ(~）|パネルを開く(閉じる)。移動でアクティビになるので実行が簡単にできる|

## Live Share
- Live Share Extension pack をインストール
## 便利機能
- ファイルとファイルの比較(2通りある)
  - コマンドパレットからcompareを選ぶ。比較するファイルを選択するとコードが変わるところがわかる
  - 選択するファイルを`cmd + ファイルを押す`次に右クリックで`選択項目の比較`を選ぶ
- 同じ文字列の選択
  - 任意の文字列を選択して、\[ctrl] + \[shift] + \[L] を押す
  - 文字の書き換えもできる
- エディタとターミナルの移動
  - パネルで`🔼`パネルサイズの最大化を押す
  - ctrl + ` でエディタとターミナルを切り替える
## 機能
- ユーザースニペット
- task
- デバッガ
- git & github & github Actions
- test
- 仮想環境
- ライブラリの作成

## 参考
- setting.jsonの保存場所
  - /Users/Username/Library/Application Support/Code/User `cd "Application Support"`で移動
