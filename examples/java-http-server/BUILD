target(
    dependencies = [
        "finatra/examples/java-http-server/src/main/java",
    ],
)

target(
    name = "tests",
    dependencies = [
        "finatra/examples/java-http-server/src/test/java",
    ],
)

jvm_binary(
    name = "bin",
    basename = "java-http-server",
    main = "com.twitter.hello.server.HelloWorldServerMain",
    dependencies = [
        ":java-http-server",
        "3rdparty/jvm/ch/qos/logback:logback-classic",
    ],
    deploy_excludes = [
        exclude("org.slf4j", "slf4j-jdk14"),
        exclude("log4j", "log4j"),
    ],
)
