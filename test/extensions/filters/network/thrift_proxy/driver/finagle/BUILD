load("@rules_python//python:defs.bzl", "py_library")
load("//bazel:envoy_build_system.bzl", "envoy_package")
load("@thrift_pip3//:requirements.bzl", "requirement")

licenses(["notice"])  # Apache 2

envoy_package()

py_library(
    name = "finagle_lib",
    srcs = [
        "TFinagleServerProcessor.py",
        "TFinagleServerProtocol.py",
        "__init__.py",
    ],
    deps = [
        "@com_github_twitter_common_finagle_thrift//:twitter_common_finagle_thrift",
        "@com_github_twitter_common_rpc//:twitter_common_rpc",
        requirement("thrift"),
    ],
)
