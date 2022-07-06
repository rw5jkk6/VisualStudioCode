## bind mount
- ディレクトリがない場合
  - `docker run -it -rm --name コンテナ名 -v "$(pwd)":/コンテナで作るディレクトリ名 イメージ名`
