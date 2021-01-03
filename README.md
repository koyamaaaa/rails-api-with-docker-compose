## Initialize rails app with api-mode and mysql

```sh
$ docker-compose run web rails new . --api --force --database=mysql
```

## Create DB

```sh
  $ docker-compose run web rails db:create
```

## DB migration

### Create migration

```sh
  $ docker-compose run web rails g migration MIGRATION_NAME
```

### Migrate

```sh
  $ docker-compose run web rails db:migrate
```

## Access DB

### Access DB Container

```sh
  $ docker exec -it DB_CONTAINER_NAME bash
```

### Access DB in DB Container

```sh
  $ mysql -u root -p SETTING_PASSWORD
```

## Execute rspec

```sh
  $ docker-compose run web bundle exec rspec
```

[rspec/rspec-rails](https://github.com/rspec/rspec-rails)

## Execute rubocop

```sh
  $ docker-compose run web rubocop
```

[rubocop-hq/rubocop](https://github.com/rubocop-hq/rubocop)
