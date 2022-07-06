## Dockerの基本的な使い方
- コンテナの削除
  - `docker container rm -f コンテナ名` 
- image削除
  - `docker image ls -q | xargs docker image rm -f`
  - -q  
