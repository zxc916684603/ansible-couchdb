# 服务启停

使用由Websoft9提供的 CouchDB 部署方案，可能需要用到的服务如下：

## CouchDB

```shell
sudo systemctl start couchdb-server
sudo systemctl stop couchdb-server
sudo systemctl restart couchdb-server
sudo systemctl status couchdb-server

# you can use this debug mode if CouchDB service can't run
couchdb-server console
```

### MySQL

```shell
sudo systemctl start mysql
sudo systemctl stop mysql
sudo systemctl restart mysql
sudo systemctl status mysql
```

### Redis

```shell
systemctl start redis
systemctl stop redis
systemctl restart redis
systemctl status redis
```