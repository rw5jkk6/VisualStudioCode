## aptでインストールするGoはバージョンは古いので自分で入れる
- Goのバージョンを調べる
  - `go version` 
- aptを更新
  - `sudo apt update`
- 古いGoを削除する
  - `sudo apt remove golang-go`
  - `sudo apt remove --auto-remove golang-go`
  - `sudo apt purge golang*`

- Goのインストールのサイト
  - https://go.dev/doc/install 
- Goを公式サイトからダウンロードする
  - `wget https://go.dev/dl/go1.19.linux-amd64.tar.gz` 


![IMG_2741](https://user-images.githubusercontent.com/66894552/183646108-fa11f004-d663-4811-9274-5c978ed63bb9.JPG)
