load("@io_bazel_rules_go//go:def.bzl", "go_prefix", "go_test")
load("@io_bazel_rules_go//tests:bazel_tests.bzl", "bazel_test")

go_prefix("github.com/bazelbuild/rules_go")

go_test(
    name = "go_default_test",
    size = "small",
    srcs = ["test_filter_test.go"],
    tags = ["manual"],
)

bazel_test(
    name = "test_filter_test_1.7.5",
    command = "test",
    args = ["--test_filter=Pass"],
    target = "//:go_default_test",
    go_version = "1.7.5",
    tags = ["dev"],
)
