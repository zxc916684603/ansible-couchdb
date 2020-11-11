# FAQ


#### Can I reset password of CouchDB by command?

No，Log in to CouchDB web console,Set you new password from: 【Users】
![](https://libs.websoft9.com/Websoft9/DocsPicture/en/couchdb/couchdb-pw-websoft9.png)

#### If there is no domain name, can I deploy CouchDB?

Yes, visit CouchDB by *http://Internet/_utils*

#### What is the password for the database root user?

The password is stored in the server related file: `/credentials/password.txt`

#### Is there a web-base GUI database management tools?

Yes,  visit CouchDB by *http://Internet/_utils*

#### Is it possible to modify the source path of CouchDB?

No

#### How to change the permissions of filesytem?

Change owner(group) or permissions like below:

```shell
chown -R apache.apache /data/wwwroot
find /data/wwwroot -type d -exec chmod 750 {} \;
find /data/wwwroot -type f -exec chmod 640 {} \;
```

#### What's the difference between Deployment and Installation?

- Deployment is a process of installing and configuring a sequence of software in sequence in a different order, which is a complex system engineering.  
- Installation is the process of starting the initial wizard after the application is prepared.  
- Installation is simpler than deployment. 

#### What's Cloud Platform?

Cloud platform refers to platform manufacturers that provide cloud computing services, such as: **Azure, AWS, Alibaba Cloud, HUAWEI CLOUD, Tencent Cloud**, etc.

#### How backing up CouchDB？

CouchDB has three different types of files it can create during runtime:Database files，Configuration files，Log files 
Refer to the official docs：[Backing up CouchDB](https://docs.couchdb.org/en/latest/maintenance/backups.html)


#### What is the difference between Instance, Cloud Server, Virtual Machine, ECS, EC2, CVM, and VM?

No difference, just the terminology used by different manufacturers, actually cloud servers