# GOでAPIサーバー作る

## 構成
- go.mod: Goのモジュールパスを書いておくファイル。モジュールの中に含まれる全てのパッケージインポート用のパスプレフィックスが書かれている。
- go.sum: 直接・間接を問わず依存先モジュールのハッシュを記録するためのファイルです。取得されたモジュールのハッシュと、こちらに記載されたハッシュが食い違うとエラーを検知することができるという、モジュールのバージョンをチェックするのに役立つファイル。これ自体はなくても、ビルドの再現はできる。

## ローカル実行環境の構築
1. GOのインストール: `go version go1.17.5 darwin/amd64`
```
brew install go
```
2. ルートディレクトリ直下で、サーバー起動
```
go run main.go
```
