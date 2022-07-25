## PullRequestする方法は３通りある
1. VSCodeのアイコンをクリック
2. ウェブサイトのGitHub
3. ターミナルのコマンドライン

![IMG_0185](https://user-images.githubusercontent.com/66894552/179152820-5f97a0c3-d9f8-4961-be46-93b8c9991c5e.PNG)

## 1. Pull Request(VSCode)
- originがないと同期できないので、Githubのバージョン管理していないと使えないので注意
- forkする。forkすると自分と相手側と同じレポジトリ名のが２つ作られるが自分のリポジトリでしなければならないので注意
- 最新のコードに更新(以下のどちらか)
  - git pull origin master
  - git clone
- branchを作ってbranchに移動(branchを作らないとPull Requestができないので注意)
  - vscodeの左下の画面でブランチを切り替える 
- コードを加筆または修正する
- ステージングしてメッセージをつけてコミット
- リモートにpush
- ここからGitHubのサイトで
- 自分のGithub上でpull requestタブを押す
- Codeタブで`commit & pull request`で押す
- タイトルとコメントを入れて`create pull request`を押す
## 2. Pull Request(Github)
- ここは全てGitHubのウェブサイトで行う
- forkする。forkすると自分と相手側と同じレポジトリ名のが２つ作られるが自分のリポジトリでしなければならないので注意
- コードを加筆または修正する。
- 同じページの下の方に変更のメッセージを書いて`Create a new branch ~~ `に変えて、ボタンの`Propose changes`を押す
- pullRequestタブを押す

## 3. Pull Request(ターミナルでコマンド)

- ブランチの確認
- `git branch`
- `git pull origin master`
- `git status`
- `git checkout -b ブランチ名`
- ファイルの変更
- `git add ファイル名`
- `git commit` vimが開くので、コメントを書く。終了は　`:wq`
- `git push origin レポジトリ名` この時点では、まだ自分のGitHubは書き換えられない。
- ここからGitHubのサイトで(上のvscodeの時と同じ)
- 自分のGithub上でpull requestタブを押す
- Codeタブで`commit & pull request`で押す
- タイトルとコメントを入れて`create pull request`を押す
