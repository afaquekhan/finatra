target(
    dependencies = [
        "finatra/examples/twitter-clone/src/main/scala",
    ],
)

target(
    name = "tests",
    dependencies = [
        "finatra/examples/twitter-clone/src/test/scala",
    ],
)

jvm_binary(
    name = "bin",
    basename = "finatra-twitter-clone",
    main = "finatra.quickstart.TwitterCloneServerMain",
    dependencies = [
        ":twitter-clone",
        "3rdparty/jvm/ch/qos/logback:logback-classic",
    ],
    excludes = [
        exclude("org.slf4j", "slf4j-jdk14"),
        exclude("log4j", "log4j"),
    ],
)
