
# flyway-gradle hands on

## setup

```
mysql-ctl start
mysql -u root < create_db.sql
```

## 1 basic

### info

```
cd 1-basic
./gradlew flywayInfo
```

### migrate

```
./gradlew flywayMigrate
```

## 2 existing

### info

```
cd 1-basic
./gradlew flywayInfo
```

### migrate

```
./gradlew flywayMigrate
```

### baseline

```
./gradlew flywayBaseline
```

```
./gradlew flywayMigrate
```

## 3 repair

```
./gradlew flywayMigrate
```

SQL ERROR...

```
./gradlew flywayRepair
```

```
./gradlew flywayInfo
```

- Pending
- fix ddl

```
./gradlew flywayMigrate
```

## 4 reset

```
DROP TABLE ...
/* fix version manually */
DELETE FROM schema_version WHERE id = ?
```

```
./gradlew flywayInfo
```




