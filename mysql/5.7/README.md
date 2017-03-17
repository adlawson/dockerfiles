# MySQL 5.7

This image builds upon the official MySQL 5.7 image by adding `less` for paging.

```bash
> docker build -t adlawson/mysql:5.7 .
```

```bash
> alias mysql="docker run --rm -it \
    -v $HOME/.my.cnf:/etc/mysql/conf.d/my.cnf \
    adlawson/mysql:5.7 mysql"

> mysql -h127.0.0.1 -P3306 -umyuser -p
```
