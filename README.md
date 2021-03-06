
![image](https://github.com/wenbo2018/Jconf/blob/master/resources/new_log.jpeg)



## Jconf
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=102)](https://github.com/wenbo2018/fox/)


Jconf is a distributed configuration management platform.Jconf provides centralized management of configuration, and the configuration 
changes are immediately synchronized to the client.You can use Jconf API directly in the code configuration, In spring, you can use spring
 placeholders for direct configuration without the need to configure the read problem.

## Maven dependency

### latest release version is 1.0.0

```xml
    <dependency>
        <groupId>com.github.wenbo2018</groupId>
        <artifactId>jconf-client-sdk</artifactId>
        <version>1.0.0</version>
    </dependency>

```

# Quick Start

1.Configure configuration center address,you need to configure the following files in the specified folder。

/data/app/jconf.properties(Linux),C:/data/app/jconf.properties(Win)

```xml
jconf.properties:zookeeper.register.address=170.0.0.1,170.0.0.2,170.0.0.3

```
2.Add Maven dependency with latest release version.

3.Configuring in Spring

```xml
    <bean class="com.github.wenbo2018.jconf.client.spring.JconfigSpringSupport"/>
```

# Jconf-admin-web Start

Jconf provides a background management system for centralized management of your configuration that is jconf-admin-web,jconf-admin-web was developed by Spring BOOT.You can make it easy to run.


```xml

git clone git@github.com:wenbo2018/Jconf.git

cd Jconf/jconf-admin-web

mvn mvn package

java -jar xxx.jar

http://localhost:9000/jconf/wel
 
check Jconf Application started!

```

Jconf web admin
==================================
 ![image](https://github.com/wenbo2018/Jconf/blob/master/resources/newUI.jpeg)

##  License

Licensed to the Apache Software Foundation (ASF) under one or more contributor license agreements. See the NOTICE file distributed with this work for additional information regarding copyright ownership. The ASF licenses this file to you under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
