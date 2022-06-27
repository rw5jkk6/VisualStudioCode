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
## 練習
- lifeフォルダを作る
- アクティビティバーからgitマークを選んでリポジトリを初期化する
- 学生の章
  - hitoshi.txtに`高校を卒業する`と書いて、commitする
  - hitoshi.txtに`大学を卒業する`と書いて、commitする
  - さっきのcommitを取り消す(revert)
  - hitoshi.txtに`大学に入学する`と書いて、commitする
  - hitoshi.txtに`大学を卒業する`と書いて、commitする
  - 上のcommitに対して、`age22`というタグをつける
- 卒業後の章
  - branch-dentuを作る
  - hitoshi.txtに`電通に就職する`と書いて、commitする
  - hitoshi.txtに`全然ついていけないので3日で辞める`と書いて、commitする

- gitマークを選んでサイドバーの上にあるgit graphを見てみる
- git graphでmasterの横のコメントで右クリックしてcreate branchを押す
- branch-tacを作って、check　outにチェックマークしてcreate Branchを押す
- hitoshi.txtに`tacに入る`と書く、commitする
- hitoshi.txtに`何年やっても全然わからん`と書いて、commitする
- tacが一番マシなのでtacをmergeする。masterにcheckoutして、brach-tacで右クリックしてを\[Merge into current branch ...]を選択する
