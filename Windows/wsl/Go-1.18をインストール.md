## aptでインストールするGoはバージョンは古いので自分で入れる
- Goのバージョンを調べる
  - `go version` 
- aptを更新
  - `sudo apt update`
- 古いGoを削除する
  - `sudo apt remove golang-go`
  - `sudo apt remove --auto-remove golang-go`
  - `sudo apt purge golang*`

- Goを公式サイトからダウンロードする
  - `wget https://dl.google.com/go/go1.18.linux-amd64.tag.gz` 


![IMG_2741](https://user-images.githubusercontent.com/66894552/183646108-fa11f004-d663-4811-9274-5c978ed63bb9.JPG)
