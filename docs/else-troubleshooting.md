# Troubleshooting

We collect the most common troubleshooting of using CouchDB for your reference:

#### How can I use the logs?

You can find the keywords **Failed** or **error** from the logs directory: `/data/logs`

#### CouchDB service can't start?

1. Use the debug mode of `couchdb-server console` and you can see the errors
   ```
   couchdb-server console
   ```
2. Search the keywords **Failed** or **error** from logs: */data/logs/couchdb-server*

#### Error in Chrome when modify password?

This error is not attribute to CouchDB server, once you have upgraded you local Chrome, it solved

![chrome error of CouchDB](https://libs.websoft9.com/Websoft9/DocsPicture/zh/couchdb/couchdb-chromeerror-websoft9.png)