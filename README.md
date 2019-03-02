# 概要
とにかくサクっとPHP+MySQLで開発環境が作りたい人向け。(Linux Mintで動作確認)
VSCodeでリモートデバッグするためのlaunch.jsonも同梱しています。

# 事前準備
docker と docker-compose をインストールしてPATHを通している状態にする。

```
$ sudo apt-get install docker
$ sudo apt-get install docker-compose
```

# 使い方
1. git clone する
2. Dockerを立ち上げる
```
$ cd docker-php-base/docker
$ docker-compose up
```
3. VSCode でdocker-php-baseディレクトリを開く
4. src/mysql-test.php の5行目などでブレイクポイントを設定しておく
5. F5でデバッグを起動
6. http://localhost/mysql-test.php にアクセスしてブレイクすればリモートデバッグ成功
