load("@aspect_bazel_lib//lib:copy_to_bin.bzl", "copy_to_bin")
load("@npm//:defs.bzl", "npm_link_all_packages")
load("@aspect_rules_js//npm:defs.bzl", "npm_link_package")

package(default_visibility = ["//visibility:public"])

npm_link_package(
    name = "node_modules/@myorg-js/util",
    src = "//myorg/js/util:pkg",
    visibility = ["//visibility:public"],
)

npm_link_all_packages(name = "node_modules")

copy_to_bin(
    name = "tsconfig.base",
    srcs = ["tsconfig.base.json"],
    visibility =["//visibility:public"],
)
