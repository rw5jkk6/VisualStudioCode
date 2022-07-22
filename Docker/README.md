## Dockerの基本的な使い方
- 基本的な立ち上げ方
  - `docker container run -it --name "test" alpine`
- 一時退出
  - `ctrl + p, ctrl + q`
- hostからコンテナにコピー
  - `docker container cp ホスト コンテナ名:コンテナのディレクトリ`
- コンテナに接続
  - docker container attach コンテナ名
- コンテナの削除
  - `docker container rm -f コンテナ名` 
- image削除
  - `docker images ls -q | xargs docker image rm -f`
    - -q イメージidのみを表示する  
- コンテナの削除
  - `docker container ls -q | xargs docker container rm -f`
## Dockerfileからイメージを作る
- `docker build -t イメージ名:tag . `
