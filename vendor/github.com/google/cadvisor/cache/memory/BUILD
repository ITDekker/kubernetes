load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["memory.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/google/cadvisor/cache/memory",
    importpath = "github.com/google/cadvisor/cache/memory",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/google/cadvisor/info/v1:go_default_library",
        "//vendor/github.com/google/cadvisor/storage:go_default_library",
        "//vendor/github.com/google/cadvisor/utils:go_default_library",
        "//vendor/k8s.io/klog:go_default_library",
    ],
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
