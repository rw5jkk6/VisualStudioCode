## 応用 
- gitのバージョン管理を使う
  - masterでAddを作る
  - branchでSubを作る
  - masterにbranchをマージする

- testを書く
  - ライブラリのテストを書く。main.goがないので、テストを書かないと正確性が検証できない
  - GitHubActionsを使う 

## コマンド
- commit
  - サイドバーの+ボタンでステージングしてコメントを書いてcommand + enterを押す
- revert
  - commitを取り消す。○masterの右のとこで右クリックしてrevert..を押す。commitすることで削除される
  - `Revert "コメント"`と表示される
- tag
  - タグをつける。何かしらの印をつけておくため。公開用やtestなどつけておく 
- branch
  -  

## 事前準備
- 拡張機能で git graph を入れる
## 練習(各章は独立している)
- lifeフォルダを作る
- アクティビティバーからgitマークを選んでリポジトリを初期化する
- 学生の章
  - hitoshi.txtに`高校を卒業する`と書いて、commitする
  - hitoshi.txtに`大学を卒業する`と書いて、commitする
  - さっきのcommitを取り消す(revert)
  - hitoshi.txtに`大学に入学する`と書いて、commitする
  - hitoshi.txtに`大学を卒業する`と書いて、commitする
  - 上のcommitに対して、`age22`というタグをつける

- 予定の章
  - 新しいフォルダを作ってgitを初期化する 
  - `ひとしは`をcommitする
  - `10年後プログラミングをマスターする`と書いてcommitする 
  - git graphを起動する
  - 一番初めのところでbranchを作って、checkoutする
  - `1年後プログラミングをマスターする`と書いてcommitする
  - masterにcheckoutする。vscodeの左下のbranchをmasterにする
  - branchの右のとこで右クリックしてmergeする
  - dismissというコンフリクトが起こる。上と下で比較が書いてあるので、下のAccept Incoming Changeを選ぶ
  - ステージングしてcommitする

- gitマークを選んでサイドバーの上にあるgit graphを見てみる
- git graphでmasterの横のコメントで右クリックしてcreate branchを押す
- branch-tacを作って、check　outにチェックマークしてcreate Branchを押す
- hitoshi.txtに`tacに入る`と書く、commitする
- hitoshi.txtに`何年やっても全然わからん`と書いて、commitする
- tacが一番マシなのでtacをmergeする。masterにcheckoutして、brach-tacで右クリックしてを\[Merge into current branch ...]を選択する

## 事前準備
- 拡張機能で git graph を入れる
## 練習
- culcフォルダを作る
- アクティビティバーからgitマークを選んでリポジトリを初期化する
- main.goファイルにadd関数を作って表示するコードを書く
- サイドバーの+ボタンでステージングしてコメントを書いてcommand + enterを押してcommitする
- 上と同じようにして、sub関数を作って、commitする
- gitマークを選んでサイドバーの上にあるgit graphを見てみる
- git graphでmasterの横のコメントで右クリックしてcreate branchを押す
- branch-mulを作って、check　outにチェックマークしてcreate Branchを押す
  - 関数mulを作ってcommitする 
- masterに戻ってbranch-mulを右クリックしてを\[Merge into current branch ...]を選択する
