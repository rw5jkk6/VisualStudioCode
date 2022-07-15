## binフォルダにpathを通す。(環境変数の設定)
- /Userの直下に`bin`フォルダを作る
- 例えばGoでHello worldを表示するアプリを作る
- USERの直下にある` ~/.bash_profile`フォルダをvimで開く
- vimで一番下の行に加筆する
  - `export PATH="$PATH:$HOME/bin"` 
  - 上の説明 exportは環境変数に追加するコマンド、
