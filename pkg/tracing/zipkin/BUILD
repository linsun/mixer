package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["recorder.go"],
    visibility = ["//visibility:public"],
    deps = [
        "@com_github_golang_glog//:go_default_library",
        "@com_github_openzipkin_zipkin_go_opentracing//:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    size = "small",
    srcs = ["recorder_test.go"],
    library = ":go_default_library",
    deps = [
        "@com_github_golang_glog//:go_default_library",
        "@com_github_openzipkin_zipkin_go_opentracing//:go_default_library",
        "@com_github_openzipkin_zipkin_go_opentracing//types:go_default_library",
    ],
)
