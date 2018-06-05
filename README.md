# setting_gce_memo

- GCE作成

  参考
  https://qiita.com/ndxbn/items/7ef0a96e409a5b5837bd

- sshログイン

- 鍵作成

  ssh-keygen -t rsa

- nodejsインストール

  anyenv + nodenvを利用

  git clone git@github.com:yfujii01/install_setting.git

- expressでサーバー立て

  git clone git@github.com:yfujii01/minimumServer.git

- ファイアウォール設定

  GCPの設定画面 > VPCネットワーク > ファイアウォール ルール

  ファイアウォール ルールを作成

  以下の設定を行う

  |設定名|値|
  |---|---|
  |送信/受信|上り|
  |ターゲットタグ|http-server|
  |IP範囲|0.0.0.0/0|
  |プロトコルとポート|tcp:3000|
