## 事前準備
- Goで`Hello world`を出力するファイル名`hello`アプリを作る。
- 実行する

## 知っておくべきkeyword
- export
- printenv
- cp
- mv
- $HOME
- $PATH
- .bash_profile

![IMG_2713](https://user-images.githubusercontent.com/66894552/179349866-50f14db9-c1e5-4da7-8591-d3fe7a503819.JPG)

## PATHを通す目的
- コマンドをどこからでも呼び出すことができるフォルダを作る

## binフォルダにpathを通す。(環境変数の設定)
- /Users/ユーザーネームの直下に`bin`フォルダを作る
- 例えばGoでHello worldを表示するアプリを作る
- 念のため`.bash_profile`を消しても大丈夫のため保存しておく
  - ホームディレクトリに移動
  - `cp .bash_profile $HOME/Desktop`
  - `mv ./bash_profile save_bash_profile`
- USERの直下にある` ~/.bash_profile`フォルダをvimで開く
- vimで一番下の行に加筆する
  - `export PATH="$PATH:$HOME/bin"` 
  - 上の説明 exportは環境変数に追加するコマンド、
