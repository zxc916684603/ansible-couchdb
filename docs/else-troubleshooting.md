# Troubleshooting

We collect the most common troubleshooting of using CouchDB for your reference:

#### How can I use the logs?

You can find the keywords **Failed** or **error** from the logs directory: `/data/logs`

#### CouchDB service can't start?

1. Execute `systemctl status couchdb` and you can see the errors

2. Search the keywords **Failed** or **error** from logs: */data/logs/couchdb-server*

#### Error in Chrome when modify password?

This error is not attribute to CouchDB server, once you have upgraded you local Chrome, it solved