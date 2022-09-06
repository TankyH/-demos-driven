load("@rules_java//java:defs.bzl", "java_binary", "java_library")

java_library(
    name = "java-maven-lib",
    srcs = glob(["demo/guice/GuiceDemo.java"]),
    deps = [
        "@maven//:com_google_inject_guice",
        "@maven//:javax_inject_javax_inject",
    ],
)

java_binary(
    name = "guicedemo",
    main_class = "demo.guice.GuiceDemo",
    runtime_deps = [":java-maven-lib"],
)
