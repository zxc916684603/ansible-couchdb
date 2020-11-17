# More

Each of the following solutions has been proven to be effective and we hope to be helpful to you.

## Configuration 

Refer to the official docs: https://docs.couchdb.org/en/latest/config/index.html

## Domain binding

The precondition for binding a domain is that CouchDB can accessed by domain name.

Nonetheless, from the perspective of server security and subsequent maintenance considerations, the **Domain Binding** step cannot be omitted.

CouchDB domain name binding steps:

1. Connect your Cloud Server
2. Modify [Nginx vhost configuration file](/stack-components.md#nginx), change the **server_name**'s value to your domain name
   ```text
   server
   {
   listen 80;
   server_name www.example.com;  # 此处修改为你的域名
   index index.html index.htm index.php;
   root  /data/wwwroot/www.example.com;
   ...
   }
   ```
## Enable the MongoDB remote connection

1. Use **SSH** to connect CouchDB server and modify the CouchDB configuration file: */opt/couchdb/etc/default.ini*
   ```
   #1 set bindIP to 0.0.0.0
      #bind_address = 127.0.0.1
      bind_address = 0.0.0.0
   ```
   > 0.0.0.0 means any Internet IP can connect your CouchDB

2. Restart CouchDB service
   ```
   systemctl restart couchdb
   ```


## Password management

Reset password is the process of resetting a new password through special solutions in case the password has been forgotten.

1. Use **SSH** to connect CouchDB server and modify the CouchDB configuration file: */opt/couchdb/etc/local.ini*
   ```
   admin = $new_password
   ```
2. Restart the CouchDB service
   ```
   systemctl restart couchdb
   ```
