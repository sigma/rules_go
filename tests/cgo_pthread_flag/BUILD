load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["cgo_pthread_flag.go"],
    cgo = True,
)

go_test(
    name = "go_default_test",
    size = "small",
    srcs = ["cgo_pthread_flag_test.go"],
    library = ":go_default_library",
)
