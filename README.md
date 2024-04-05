# Billcat Maven Archetypes

```
net.billcat.archetypes
├── simple-jar
├── simple-boot3
├── simple-pom
├── multi-module-boot3
├── multi-module-cloud
├── multi-module-cloud-alibaba
├── multi-module-cloud-k8s
└── submodule
```

## Getting started

```shell
git clone git@github.com:billcat-projects/billcat-maven-archetypes.git
cd billcat-maven-archetypes
mvn clean install
```

From command line.

```shell
mvn archetype:generate \
-DarchetypeGroupId=net.billcat.archetypes \
-DarchetypeArtifactId=simple-jar \
-DarchetypeVersion=1.0.0
```
Or use it from IJ IDEA:



## 鸡生蛋还是蛋生鸡

本项目

1. 父模块使用 IJ 的 `maven-archetype-quickstart` 创建(建好后删除 src 目录), 项目类型为 `pom`
2. 子模块使用 IJ 的 `maven-archetype-archetype` 创建( 注意版本号要修改为 `1.4`), 项目类型为 `maven-archetype`

也可以使用命令行:

```shell
mvn archetype:generate \
-DarchetypeGroupId=org.apache.maven.archetypes \
-DarchetypeArtifactId=maven-archetype-archetype \
-DarchetypeVersion=1.4
```

## 项目完成后

父子模块都可以使用本项目的产物创建.


## License

[Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.html) .

Copyright (c) The Billcat Authors. 
