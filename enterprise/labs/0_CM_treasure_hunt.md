
```CM Monitoring Lab```

What is uber task optimization?

To Run “sufficiently small” jobs sequentially within a single JVM. This property can be changed in Performance category. 
Property name is mapreduce.job.ubertask.enable 

Where in CM is the Kerberos Security Realm value displayed?

In the Cloudera Manager Admin Console, select Administration > Settings.
Click the Security category, and enter the Kerberos realm for the cluster in the Kerberos Security Realm field (for example, YOUR-LOCAL-REALM.COM or YOUR-SUB-REALM.YOUR-LOCAL-REALM.COM) that you configured in the krb5.conf file.


How do you upgrade the CM agents?

1)sudo service cloudera-scm-agent stop
2)Copy the appropriate repo file as described in Upgrade Cloudera Manager Server (Packages).
3)$ sudo yum clean all $ sudo yum upgrade cloudera-manager-server 
cloudera-manager-daemons cloudera-manager-server-db-2 cloudera-manager-agent
4)sudo service cloudera-scm-agent start

Give the tsquery statement used to chart Hue's CPU utilization?

select * where roleType=HIVEMETASTORE
or
select * where roleType=HIVESERVER2,


Name all the roles that make up the Hive service?

Hive (Service-Wide)
Gateway
Hive Metastore Server
HiveServer
WebHCat Server

What steps must be completed before integrating Cloudera Manager with Kerberos?

We need to have a working Kerberos key distribution center (KDC) and realm setup, and we should have installed the 
Kerberos client packages on all cluster hosts and hosts that will be used to access the cluster. 
Furthermore, Oozie and Hue require that the realm support renewable tickets


```CM Lab```




