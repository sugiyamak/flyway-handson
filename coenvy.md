

## Workspace作成

![](img/1.png)

- `Add Workspace` をクリック

![](img/2.png)

- `java-MySQL` を選択

![](img/3.png)

- `Git` にこのリポジトリのURL( https://github.com/vertical-blank/flyway-handson.git )をペーストし`Add`を押す

![](img/4.png)

- `Create` を押ししばし待つ

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
cd flyway-handson
mysql -h db -u root -p < create_db.sql
```

