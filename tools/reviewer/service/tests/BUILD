package(default_visibility = ["//visibility:public"])

java_binary(
    name = "test_tool",
    srcs = [
        "TestTool.java",
    ],
    main_class = "com.google.startupos.tools.reviewer.service.tests.TestTool",
    deps = [
        "//common",
        "//common/repo:repo_java_proto",
        "//third_party/maven/io/grpc:grpc_core",
        "//third_party/maven/io/grpc:grpc_netty",
        "//third_party/maven/org/slf4j:slf4j_simple",
        "//tools/reviewer/service",
        "//tools/reviewer/service:code_review_java_grpc",
        "//tools/reviewer/service:code_review_java_proto",
    ],
)

java_test(
    name = "CodeReviewServiceTest",
    srcs = [
        "CodeReviewServiceTest.java",
    ],
    local = 1,
    test_class = "com.google.startupos.tools.reviewer.service.tests.CodeReviewServiceTest",
    deps = [
        "//common",
        "//common:dagger_with_annotation_processor",
        "//common:text_differencer",
        "//common/flags",
        "//common/repo",
        "//common/repo:repo_java_proto",
        "//third_party/maven/com/google/flogger",
        "//third_party/maven/com/google/flogger:flogger_system_backend",
        "//third_party/maven/com/google/guava",
        "//third_party/maven/io/grpc:grpc_core",
        "//third_party/maven/io/grpc:grpc_netty",
        "//third_party/maven/io/grpc:grpc_services",
        "//third_party/maven/junit",
        "//third_party/maven/org/mockito:mockito_core",
        "//third_party/maven/org/objenesis",
        "//tools/aa:aa_module",
        "//tools/aa/commands",
        "//tools/local_server/service:auth_service",
        "//tools/reviewer/service",
        "//tools/reviewer/service:code_review_java_grpc",
        "//tools/reviewer/service:code_review_java_proto",
    ],
)
