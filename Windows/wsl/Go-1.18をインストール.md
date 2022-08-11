## aptでインストールするGoはバージョンは古いので自分で入れる
- Goのバージョンを調べる
  - `go version` 
- aptを更新
  - `sudo apt update`
- 古いGoを削除する
  - `sudo apt remove golang-go`
    - パッケージを削除する 
  - `sudo apt remove --auto-remove golang-go`
    - 依存のパッケージ関連を削除 
  - `sudo apt purge golang*`
    - purgeはGoの設定情報を消去する 

- Goのインストールのサイト
  - https://go.dev/doc/install 
- Goを公式サイトからダウンロードする
  - `wget https://dl.google.com/go/go1.18.linux-amd64.tar.gz`
  - または
  - `wget https://go.dev/dl/go1.19.linux-amd64.tar.gz` 

- Goフォルダに移動して解凍
  - `sudo tar -C /usr/local -xzf go1.18.linux-amd64.tar.gz` 
    - -C 解凍先のディレクトリの指定
    - -x アーカイブの展開
    - -z tar.gzの展開
    - -f ファイル名を指定して展開 

- PATHを通す
  - 基本は画像を参考にする
  - homeディレクトリの隠しファイルの`.profile`を開いて`code .profile`末尾に記述
    - `code .profile`とコマンドすることでvscodeで開くことができる 
    - `export PATH=$PATH:/usr/local/go/bin` 
  - .profileをリフレッシュさせる
    - `source .profile`
  - Goのバージョンの確認
    - `go version`  

![IMG_2741](https://user-images.githubusercontent.com/66894552/183646108-fa11f004-d663-4811-9274-5c978ed63bb9.JPG)

