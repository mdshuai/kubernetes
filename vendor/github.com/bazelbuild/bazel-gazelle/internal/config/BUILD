load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "config.go",
        "constants.go",
        "directives.go",
        "platform.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/bazelbuild/bazel-gazelle/internal/config",
    importpath = "github.com/bazelbuild/bazel-gazelle/internal/config",
    visibility = ["//vendor/github.com/bazelbuild/bazel-gazelle:__subpackages__"],
    deps = ["//vendor/github.com/bazelbuild/buildtools/build:go_default_library"],
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
