# Docker Microsoft SQL Server

https://docs.microsoft.com/ja-jp/sql/linux/quickstart-install-connect-docker

# 設定

ログインパスワードは`common.env`の`MSSQL_SA_PASSWORD`で設定してください


# 初期データ

init-data内にsqlファイルを配置することで名前順にロードしてくれます

# 起動

```
> docker-compose up -d
```

# 停止

```
> docker-compose stop
```

# 削除

```
> docker-compose down
```

# 永続化されたデータの削除

立ち上げ時に再度データ投入してくれます

```
> docker volume ls

DRIVER   VOLUME NAME
local    dockersqlserver_mssql-db

> docker volume dockersqlserver_mssql-db
```
