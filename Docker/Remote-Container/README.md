## Dev Containerでの起動の仕方は３通り
1. 既存のDockerイメージを使い、ひとつのコンテナを起動する
    - "image"にDockerイメージの名前とタグを指定する
2. Dockerfileを使ってビルドしたDockerイメージを使い、ひとつのコンテナを起動する
    - "Dockerfile"にDockerfileのパスを指定する
## Goで作成のサンプル
1. 拡張機能で`Remote-Containers`をinstall
2. フォルダやmain.goファイルを事前に作っておく
3. vscodeの左下の`><`を押す。open folder in Container ..
4. 作ったフォルダを選択する。　Goを選択する。versionはデフォルトの1を選択。okを押す
5. Dockerが起動する準備を始める(時間が掛かる)
6. コードが書ける状態になる
