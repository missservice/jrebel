# jrebel
1. chmod -R 777 JrebelBrainsLicenseServerforJava-1.0-SNAPSHOT-jar-with-dependencies.jar
2. java -jar JrebelBrainsLicenseServerforJava-1.0-SNAPSHOT-jar-with-dependencies.jar -p 8083 &
3. print INFO:
```
2018-07-31 13:51:54.835:INFO:oejs.Server:jetty-8.y.z-SNAPSHOT
2018-07-31 13:51:54.889:INFO:oejs.AbstractConnector:Started SelectChannelConnector@0.0.0.0:18082
License Server started at http://localhost:18082
JetBrains Activation address was: http://localhost:18082/
JRebel 7.1 and earlier version Activation address was: http://localhost:18082/{tokenname}, with any email.
JRebel 2018.1 and later version Activation address was: http://localhost:18082/{guid}(eg:http://localhost:18082/5eaf3650-844a-46d9-9362-8f23750f3f8b), with any email.
```
