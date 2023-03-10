# Read Me First
The following was discovered as part of building this project:

# Getting Started

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.4.5/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.4.5/maven-plugin/reference/html/#build-image)

### Maybe A Bug
```shell
mvn clean -U  package -DskipTests
```
> Every time cmd is executed, it will be pulled `https://maven.aliyun.com/repository/public/io/grpc/grpc-core/maven-metadata.xml`
>
> when multiple projects pull `io/grpc/grpc-core/maven-metadata.xml` at the same time、 maven will be hung!