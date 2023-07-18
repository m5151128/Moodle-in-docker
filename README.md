# Moodle-in-docker

## 起動方法

```
$ docker compose up
```

※ 初回起動は時間が掛かります。

## アクセス

http://localhost:8080/

ログイン情報
- user: `user`
- password: `bitnami`

変更したい場合は[bitnami/containers](https://github.com/bitnami/containers/tree/main/bitnami/moodle)を参考に<br>
`MOODLE_USERNAME`, `MOODLE_PASSWORD`等を設定する

## Postgresqlへのアクセス

```
$ docker compose exec moodle_db psql -U moodle_user -d moodle
```
