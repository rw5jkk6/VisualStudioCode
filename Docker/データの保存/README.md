## bind mount
- ディレクトリ(ホスト側に)がない場合
  - `docker run -it -rm --name コンテナ名 -v "$(pwd)":/コンテナのディレクトリ名 イメージ名`
- ディレクトリがある場合
  - `docker run -it --name コンテナ名 --mount type=bind,source="$(pwd)",target=/コンテナのディレクトリ イメージ名` 
