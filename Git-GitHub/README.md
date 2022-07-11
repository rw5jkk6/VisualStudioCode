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
|git init|初期化する|
|git branch|ブランチを作る|
|git checkout|切り替える|
|git add (-A)|ステージング|
|git commit (-a)|コミットする|
|git diff|今のファイルとステージングされたファイルを比較する|
|git commit --amend -m "コメント"|直前の間違ったコメントを修正する|
|git fetch|更新された情報をチェックする|
|git pull|更新された情報をローカルにダウンロードする|
|git pull request|コードの変更を求める|
|git revert|過去のコミットを削除する|

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


## リモートリポジトリの複製(Gitのclone)
- リポジトリのwebページからURLを取得する
  - code　->　httpsからURLをコピーする
- vscode
  - コマンドパレットから git clone を選んでURlを貼り付ける
  - フォルダを選択または新規で作ると、そこにリポジトリのコードがダウンロードされる
## 更新されたコードをダウンロードする(pull)
- \[...]を押して \[プル、プッシュ]の右側の \[プル]を押す
- 自分のリポジトリのURLをコピーして貼り付ける
