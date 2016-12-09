
````
Ajits-MacBook-Air:Downloads ajitkumaramit$ ssh -i "Cloudera.pem" root@ec2-54-254-140-177.ap-southeast-1.compute.amazonaws.com
The authenticity of host 'ec2-54-254-140-177.ap-southeast-1.compute.amazonaws.com (54.254.140.177)' can't be established.
RSA key fingerprint is SHA256:9yfyCXNi+DwxmasJIqnG9qNOTMpzg7Vvf2WfDgPU0sA.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'ec2-54-254-140-177.ap-southeast-1.compute.amazonaws.com' (RSA) to the list of known hosts.
Last login: Fri Dec  9 01:42:42 2016 from 101.100.166.35
-bash: warning: setlocale: LC_CTYPE: cannot change locale (UTF-8): No such file or directory
[root@ip-172-31-5-17 ~]# wget http://archive.cloudera.com/cm5/redhat/6/x86_64/cm/cloudera-manager.repo
--2016-12-09 01:52:09--  http://archive.cloudera.com/cm5/redhat/6/x86_64/cm/cloudera-manager.repo
Resolving archive.cloudera.com... 151.101.8.167
Connecting to archive.cloudera.com|151.101.8.167|:80... connected.
HTTP request sent, awaiting response... 200 OK
Length: 290
Saving to: `cloudera-manager.repo'

100%[=========================================================================================>] 290         --.-K/s   in 0s      

2016-12-09 01:52:09 (28.3 MB/s) - `cloudera-manager.repo' saved [290/290]

[root@ip-172-31-5-17 ~]# ls
cloudera-manager.repo
[root@ip-172-31-5-17 ~]# mv *.repo /etc/yum.repos.d

[root@ip-172-31-5-17 ~]# cat /etc/yum.repos.d/cloudera-manager.repo
[cloudera-manager]
# Packages for Cloudera Manager, Version 5, on RedHat or CentOS 6 x86_64           	  
name=Cloudera Manager
baseurl=https://archive.cloudera.com/cm5/redhat/6/x86_64/cm/5/
gpgkey =https://archive.cloudera.com/cm5/redhat/6/x86_64/cm/RPM-GPG-KEY-cloudera    
gpgcheck = 1

[root@ip-172-31-5-17 ~]# 


````

`````````
Prepare SCM Database command

root@ip-172-31-5-17 yum.repos.d]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-5-18.ap-southeast-1.compute.internal -uroot@ip-172-31-5-18.ap-southeast-1.compute.internal -proot  --scm-host ip-172-31-5-17  scm scm scm
``````
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
2016-12-09 03:04:14,668 [main] INFO  com.cloudera.enterprise.dbutil.DbCommandExecutor  - Successfully connected to database.
All done, your SCM database is configured correctly

``````
tail -f /var/log/cloudera-scm-server/cloudera-scm-server.log


rMapping: Mapped URL path [/reports/delete-configuration.*] onto handler 'utilizationReportsController'
2016-12-09 03:06:04,279 INFO WebServerImpl:org.springframework.web.servlet.mvc.annotation.DefaultAnnotationHandlerMapping: Mapped URL path [/reports/delete-configuration/] onto handler 'utilizationReportsController'
2016-12-09 03:06:04,305 INFO WebServerImpl:org.springframework.web.servlet.handler.SimpleUrlHandlerMapping: Root mapping to handler of type [class org.springframework.web.servlet.mvc.ParameterizableViewController]
2016-12-09 03:06:04,400 INFO WebServerImpl:org.springframework.web.servlet.DispatcherServlet: FrameworkServlet 'Spring MVC Dispatcher Servlet': initialization completed in 6027 ms
2016-12-09 03:06:04,448 INFO WebServerImpl:com.cloudera.server.web.cmon.JobDetailGatekeeper: ActivityMonitor configured to allow job details for all jobs.
2016-12-09 03:06:05,262 INFO WebServerImpl:com.cloudera.server.web.cmf.AggregatorController: AggregateSummaryScheduler started.
2016-12-09 03:06:06,128 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Initializing SearchTemplateManager:2016-12-09T03:06:06.128Z
2016-12-09 03:06:06,197 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Generating entities:2016-12-09T03:06:06.197Z
2016-12-09 03:06:06,217 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Num entities:228
2016-12-09 03:06:06,217 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Generating documents:2016-12-09T03:06:06.217Z
2016-12-09 03:06:06,267 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Num docs:240
2016-12-09 03:06:06,268 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Constructing repo:2016-12-09T03:06:06.268Z
2016-12-09 03:06:06,428 INFO WebServerImpl:org.mortbay.log: jetty-6.1.26.cloudera.4
2016-12-09 03:06:06,429 INFO WebServerImpl:org.mortbay.log: Started SelectChannelConnector@0.0.0.0:7180
2016-12-09 03:06:06,429 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
2016-12-09 03:06:06,881 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Finished constructing repo:2016-12-09T03:06:06.881Z

`````


grep "Started Jetty server" /var/log/cloudera-scm-server/cloudera-scm-server.log
2016-12-09 03:06:06,429 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.

``


