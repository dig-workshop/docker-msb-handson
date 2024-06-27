## やりたい事

1. このファイルの中身を確認
2. ルート直下にあるDockerfileを起動しImageを作る
3. gradleでbuildしたSNAPSHOT.jarを openjdk:21 のイメージに渡してビルドできるようなDockerfileに書き換える
4. ビルドしたイメージの容量の差を比べてみる
5. 実際にそれぞれのイメージが動くかどうかを確認する

## 途中で使って欲しいコマンド・オプション

コマンドの一部分のみ記載しているので、必要に応じてコマンドを調整してください。

`docker image build -t hogehoge:v0.0`

`docker container run --rm -itd -p`

`docker container stop`

`docker image rm`

## 動作確認の方法

正しくイメージがビルド出来たら、それぞれのイメージをデタッチモードで起動し、ブラウザ側から指定したポートと正しいurlを用いてGETリクエストを送ってください。
