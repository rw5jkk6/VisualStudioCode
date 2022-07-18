![IMG_2684](https://user-images.githubusercontent.com/66894552/174801186-e6be4068-2301-42ff-9e5d-37306c24219e.JPG)

![IMG_2709](https://user-images.githubusercontent.com/66894552/178100079-a940f2eb-d956-41a0-acc7-e3c869f8930a.JPG)

## gitの使い方(ターミナルでなく、vscodeのサイドバーで操作する)
- リポジトリの初期化(git init)
- 変更したファイルをステージング(git add)
  - \[+] アイコンを押す 
- ファイルのコミット(git commit)
  - コメントを入力して ctrl + enter 

## gitのコマンド(カッコ()はオプション)
|コマンド|機能|
|:--|:--|
|git --version|バージョン情報|
|git config --list|設定リストの一覧表示|
|git config --global merge.ff false|FastForwardマージを禁止する|
|git init|初期化する|
|git branch|ブランチを作る|
|git checkout|切り替える|
|git add (-A　または . )|ステージング|
|git commit (-a)|コミットする|
|git diff|今のファイルとステージングされたファイルを比較する|
|git commit -m "メッセージ"|commitの際にメッセージを一緒に書く|
|git commit --amend -m "コメント"|直前の間違ったコメントを修正する|
|git fetch|更新された情報をチェックする|
|git pull|更新された情報をローカルにダウンロードする|
|git pull request|コードの変更を求める|
|git revert|過去のコミットを削除する|
|git log|commitの履歴がわかる|

## Githubでバージョン管理
- Githubでの操作
  - リポジトリを作る
  - URLをコピーしておく
- VScodeでの操作  
  - リポジトリを初期化する。一番左のアクティビティバーから作る
  - コードを書く(関数は頭は大文字)
  - git add (ステージングは + を押す)
  - git commit (コメントを入れて ctrl + enter)
  - コマンドパレットから git add remote　(リモートの追加。gitを作っておかないと出てこない)
  - GithubのリポジトリのURLを貼り付ける。リモート名は\[origin]にしておく
  - git push ソース管理ビューの...をクリックしてメニュー先の\[プッシュ先...]を選択して[origin]を選択する

## branchを使ってmergeする
- branchを作って、コードを書く
- masterにcheckoutする。GitGraphのbranchの右側を右クリックしてmergeする

## リモートリポジトリの複製(Gitのclone)
- リポジトリのwebページからURLを取得する
  - code　->　httpsからURLをコピーする
- vscode
  - コマンドパレットから git clone を選んでURlを貼り付ける
  - フォルダを選択または新規で作ると、そこにリポジトリのコードがダウンロードされる
## 更新されたコードをダウンロードする(pull)
- githubのリポジトリのコードボタン(緑色)の下に`fetch up stream`を押す。次に`fetch and merge`を押す。これで更新できる
- \[...]を押して \[プル、プッシュ]の右側の \[プル]を押す
- 自分のリポジトリのURLをコピーして貼り付ける

![IMG_0185](https://user-images.githubusercontent.com/66894552/179152820-5f97a0c3-d9f8-4961-be46-93b8c9991c5e.PNG)

## Pull Request(VSCode)
- originがないと同期できないので、Githubのバージョン管理していないと使えないので注意
- forkする。forkすると自分と相手側と同じレポジトリ名のが２つ作られるが自分のリポジトリでしなければならないので注意
- 最新のコードに更新(以下のどちらか)
  - git pull origin master
  - git clone
- branchを作ってcommit。branchを作らないとPull Requestができないので注意
- push
- 自分のGithub上でpull requestタブを押す
- Codeタブで`commit & pull request`で押す
- タイトルとコメントを入れて`create pull request`を押す
## Pull Request(Github)
- forkする。forkすると自分と相手側と同じレポジトリ名のが２つ作られるが自分のリポジトリでしなければならないので注意
- codeを編集して `Create a new branch ~~ `に変えて`Propose changes`を押す
- pullRequestタブを押す

## Pull Request(ターミナルでコマンド)

- ブランチの確認
- `git branch`
- `git pull origin master`
- `git status`
- `git checkout -b ブランチ名`
- ファイルの変更
- `git add ファイル名`
- `git commit` vimが開くので、コメントを書く。終了は　`:wq`
- `git push origin レポジトリ名` この時点では、まだ自分のGitHubは書き換えられない。
- ここからGitHubで
- `git checkout master`
- `git merge ブランチ名`
- `git pull origin master`
- `git branch -d ブランチ名`

## メモ
- masterとorigin/masterの違い
  - masterはローカルでorigin/masterはリモート
