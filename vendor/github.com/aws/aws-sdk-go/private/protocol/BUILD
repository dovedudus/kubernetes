package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "idempotency.go",
        "unmarshal.go",
    ],
    tags = ["automanaged"],
    deps = ["//vendor/github.com/aws/aws-sdk-go/aws/request:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/ec2query:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/json/jsonutil:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/jsonrpc:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/query:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/rest:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/restxml:all-srcs",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/xml/xmlutil:all-srcs",
    ],
    tags = ["automanaged"],
)
