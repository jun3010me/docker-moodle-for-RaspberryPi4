# docker-moodle-for-RaspberryPi4
Raspberry Pi 4のDockerでサクッとmoodle環境を整えたくて用意した。

## インストール方法
まずはDockerHubからbitnamiのイメージをダウンロードする。

```
docker pull bitnami/moodle
```

続いて、このリポジトリで公開しているファイルをgit cloneして、コンテナを作る。
```
git clone https://github.com/jun3010me/docker-moodle-for-RaspberryPi4
docker-compose up -d
```
これで80番ポートでアクセスすると、moodleが起動しているはず。

## ファイルの引用元
bitnamiのmoodleのイメージはこちらから。
[bitnami/moodle - Docker Image | Docker Hub](https://hub.docker.com/r/bitnami/moodle)

docker-compose.ymlはこちらから。

[docker-compose.yml](https://raw.githubusercontent.com/bitnami/containers/main/bitnami/moodle/docker-compose.yml)

Dockerfileはこちらから。

[docker composeで「moodle」を構築する | mebee](https://mebee.info/2021/05/07/post-33655/)
