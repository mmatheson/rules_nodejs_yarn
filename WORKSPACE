load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "build_bazel_rules_nodejs",
    sha256 = "9d93d4e1340c43dbf6b2fd66b683d89630a6310bf8be3bf40ec96685dcacc26c",
    urls = ["https://github.com/bazelbuild/rules_nodejs/releases/download/2.3.3/rules_nodejs-2.3.3.tar.gz"],
)

load("@build_bazel_rules_nodejs//:index.bzl", "yarn_install")

yarn_install(
    name = "npm",
    package_json = "//:package.json",
    yarn_lock = "//:yarn.lock",
)
