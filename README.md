<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
~~distributed with this work for additional information~~
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Shaded Hadoop Dependencies for Flink

<br>

This repository contains a number of shaded Hadoop dependencies for the [Apache Flink](https://flink.apache.org/) project, based on release-10.0 branch of [apache/flink-shaded](https://github.com/apache/flink-shaded/tree/release-10.0) project.

The project supports `Hadoop-2` and `Hadoop-3` , including the following shaded subprojects:

* `flink-shaded-hadoop`:  Contains the main shaded Hadoop dependenices used by Flink .
* `flink-shaded-hadoop-uber`:  Uber-shaded project of `flink-shaded-hadoop`.
* `flink-shaded-hadoop-hive`:  Contains the main shaded Hadoop and. Hive dependenices used by Flink .

<br>

##  Build Shaded Hadoop JAR

```bash
git clone https://github.com/Al-assad/flink-shaded-hadoop.git
cd ./flink-shaded-hadoop
mvn clean install
```

Default Version:

* Hadoop-3.1.1
* Hive-3.1.1

<br>

## Custom Hadoop/Hive Version

```bash

# use hadoop-3.1.0 and hive-3.1.0
mvn clean install -Dhadoop.version=3.1.0 -Dhive.version=3.1.0
```

<br>

## About

Apache Flink is an open source project of [The Apache Software Foundation](https://apache.org/) (ASF).

