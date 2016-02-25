# Krueger Cockpit

This application displays metrics exposed by standard REST endpoints in other applications. The endpoints are similar
to the ones used in the [Spring Boot Actuator][springboot] project.

# Development

For building just do

    ./gradlew

This will compile the frontend, copy over the resources and compile the backend as well.

Starting the application is as easy as:

    APPLICATION_GROUP=krueger:localhost:8080 java -jar build/libs/krueger-cockpit-fat.jar

To start the application with [Taupage (etcd)] [taupage] discovery use

    ETCD_URL=etcd.cluster.url java -jar build/libs/krueger-cockpit-fat.jar

[springboot]: http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#production-ready-endpoints "Spring Boot Actuator"
[taupage]: https://github.com/zalando-stups/taupage "Taupage"
