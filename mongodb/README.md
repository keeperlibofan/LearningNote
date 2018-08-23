### MongoDB 恢复与备份

MongoDB 3.0 的所有工具都用Go语言重新编写

```shell
> mongo --version
MongoDB shell version v3.6.3
git version: 9586e557d54ef70f9ca4b43c26892cd55257e1a5
OpenSSL version: OpenSSL 1.0.2o  27 Mar 2018
allocator: system
modules: none
build environment:
    distarch: x86_64
    target_arch: x86_64
```

#### mongodump
`sudo mongodump -h 127.0.0.1 -o /data/backups/`
就可以备份出mongo db中所有的数据

`sudo mongodump -h <host> -d fitter -o <path>`
导出指定的数据库\<db\>

#### mongorestore
mongorestore
