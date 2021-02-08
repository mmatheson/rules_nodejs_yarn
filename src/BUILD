load("@build_bazel_rules_nodejs//:index.bzl", "nodejs_binary")

package(default_visibility = ["//visibility:public"])

nodejs_binary(
    name = "app",
    data = [
        "@npm//lodash",
    ],
    entry_point = "app.js",
)
