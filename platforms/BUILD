load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["platforms.go"],
    importpath = "github.com/bazelbuild/bazelisk/platforms",
    visibility = ["//visibility:public"],
    deps = [
        "//versions:go_default_library",
        "@com_github_hashicorp_go_version//:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["platforms_test.go"],
    embed = [":go_default_library"],
)
