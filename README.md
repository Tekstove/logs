# This repo holds configuration for logs processing

| Log type          | Location                  | File pattern  |
| ----------------- |---------------------------| --------------|
| site apache logs  | filebeat-site-apache/logs | *access.log   |
| api apache logs   | filebeat-api-apache/logs  | *access.log   |

# required setup
Don't forget to increase the `vm.max_map_count=`
```
$ sysctl -w vm.max_map_count=262144
```
