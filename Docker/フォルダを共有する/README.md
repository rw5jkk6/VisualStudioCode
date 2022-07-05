- 事前にイメージを作っておいて、フォルダを共有する。
- フォルダからvscodeを起動する。
- `docker container run --rm -it --name コンテナ名 -v $(pwd):/ユーザ名 イメージ名:tag`
- vscodeでコードを書く

```dockerfile
FROM ubuntu:latest

RUN apt-get update && apt-get install -y vim gcc g++

WORKDIR /ユーザ名
```
