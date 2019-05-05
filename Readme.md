# MySQL

- MySQL version 8.0.16

## Build

```sh

docker build -t my-mysql:0.0.1 .

```

## Configure

Change password for root user if you need in `Dockerfile`.


 ```

 ENV MYSQL_ROOT_PASSWORD mysql

 ```


## Run

```sh

docker run -d -it -v "$PWD/data":/var/lib/mysql -p 3306:3306 my-mysql:0.0.1

```
## Connect From Tool

Install `MySQL Workbench` from [here](https://www.mysql.com/jp/downloads/).
And connect with the configuration below and create a database.


```
host=localhost
port=3306
user:root
password:mysql
```
