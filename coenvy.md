

## Workspace作成

![](img/1.png)

- `Add Workspace` をクリック

![](img/2.png)

- `java-MySQL` を選択

![](img/3.png)

- `Git` にこのリポジトリのURL( https://github.com/vertical-blank/flyway-handson.git )をペースト

![](img/4.png)

- しばし待つ

![](img/5.png)

- Workspace作成が完了すると、`dev-machine` のターミナルが開く
- ホスト名 `db` として、MySQLを参照可能

![](img/6.png)

- mysqlコマランドラインクライアントをインストール

```
sudo apt-get update
sudo apt-get install mysql-client -y
```

- `CREATE DATABASE` スクリプトを流す (passは `password` )
```
mysql -h db -u petclinic -p < create_db.sql
```

