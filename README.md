## Initialization

Docker on Mac

## アプリケーションのディレクトリを作成

```sh
$ mkdir YOUR_APP_NAME
```

## git clone



## initialize rails app with api-mode and mysql

```sh
$ docker-compose run web rails new . --api --force --database=mysql
```

## Create DB

```sh
  $ docker-compose run web rails db:create
```

## Access DB

### Access DB Container

```sh
  $ docker exec -it DB_CONTAINER_NAME bash
```

### Access DB

```sh
  $ mysql -u root -p SETTING_PASSWORD
```
