
```
# su - hdfs
$ hadoop fs -mkdir /user/raffles
$ hadoop fs -mkdir /user/orchard

$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred hadoop              0 2016-12-09 03:24 /user/history
drwxrwxr-t   - hive   hive                0 2016-12-09 03:25 /user/hive
drwxrwxr-x   - hue    hue                 0 2016-12-09 03:25 /user/hue
drwxrwxr-x   - oozie  oozie               0 2016-12-09 03:26 /user/oozie
drwxr-xr-x   - hdfs   supergroup          0 2016-12-09 03:25 /user/orchard
drwxr-xr-x   - hdfs   supergroup          0 2016-12-09 03:25 /user/raffles


$ curl -X GET -u  "admin:admin" -i http://ec2-54-251-167-6.ap-southeast-1.compute.amazonaws.com:7180/api/v14/hosts
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=ma9uuin0pvvi1o7v911gxo729;Path=/;HttpOnly
Content-Type: application/json
Date: Fri, 09 Dec 2016 03:30:37 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "items" : [ {
    "hostId" : "i-a03efe07",
    "ipAddress" : "172.31.5.17",
    "hostname" : "ip-172-31-5-17.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-5-18.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/i-a03efe07",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-a13efe06",
    "ipAddress" : "172.31.5.18",
    "hostname" : "ip-172-31-5-18.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-5-18.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/i-a13efe06",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-a63efe01",
    "ipAddress" : "172.31.5.19",
    "hostname" : "ip-172-31-5-19.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-5-18.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/i-a63efe01",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-a73efe00",
    "ipAddress" : "172.31.5.20",
    "hostname" : "ip-172-31-5-20.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-5-18.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/i-a73efe00",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-a43efe03",
    "ipAddress" : "172.31.5.21",
    "hostname" : "ip-172-31-5-21.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-5-18.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/i-a43efe03",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  } ]
}[hdfs@ip-172-31-5-18 ~]$ 
