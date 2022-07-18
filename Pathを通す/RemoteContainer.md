## 既存のbinを使う
- フォルダを作って、なかにDockerfileを作る。中身はココをコピーする
- VSCodeの左下の><を押して、RemoteContainerを起動する
- `Reopen in Container` 次に `From 'Dockerfile`
- main.cでHello worldを出力するアプリを作って、実行してみる。フォルダは/workspacesなので注意
- PATHをチェック`echo $PATH`
- PATHのフォルダに実行ファイルを動かす `mv /home/a.out /usr/local/bin`

## 新しいbinフォルダを作る
- ユーザフォルダにbinを作って、pathを通す
- `code .profile`でvscodeが起動できる
