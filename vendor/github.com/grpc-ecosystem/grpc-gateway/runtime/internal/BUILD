load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["stream_chunk.pb.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/grpc-ecosystem/grpc-gateway/runtime/internal",
    importpath = "github.com/grpc-ecosystem/grpc-gateway/runtime/internal",
    visibility = ["//vendor/github.com/grpc-ecosystem/grpc-gateway/runtime:__subpackages__"],
    deps = ["//vendor/github.com/golang/protobuf/proto:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
