## wslのインストール
- vscodeの設定
  - remote-wslをインストール
- ここからWindowsにWSLを入れてubuntuをインストール
- 設定を見る
  - `設定` `システム` `詳細情報` `osビルド 19041以上` 
- windowsの機能(以下にチェックを入れる)
  - Linux用 Windowsサブシステム
  - 仮想マシンプラットフォーム
- Linuxカーネルのダウンロード
  - `linux カーネル　インストール wsl`　で検索して 
  - 手順 4 の`x64 マシン用 WSL2 Linux カーネル更新プログラム パッケージ` からインストールする  
- PowerShellを開く
  - `wsl --set-default-version 2` と入力 
- Microsoft Storeからubuntuをダウンロード
  - `ubuntu`をダウンロードする。他にも`ubuntu 20.4`とかあるが、これではない
  - 開いて user名やパスワードを決める 
- ubuntuを起動して初期設定
  - `sudo apt update`
  - `sudo apt dist-upgrade -y`
  - `sudo apt install python3`

## テストでwslを使ってvscodeをPythonでHello world
- ubuntuでユーザフォルダの下にtmpフォルダを作る
- vscodeを起動する
- vscodeの左下から。新しいwslを起動するを押す
- フォルダを開くからtmpを選択
- pythonのファイルを作って、`Hello world`を作って
- 実行する

## wslのubuntuのアンインストール
- `設定` `アプリと機能` 選択したアプリのアンインストール 
