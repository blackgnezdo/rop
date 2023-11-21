load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_rust",
    sha256 = "9ecd0f2144f0a24e6bc71ebcc50a1ee5128cedeceb32187004532c9710cb2334",
    urls = ["https://github.com/bazelbuild/rules_rust/releases/download/0.29.1/rules_rust-v0.29.1.tar.gz"],
)

load("@rules_rust//rust:repositories.bzl", "rules_rust_dependencies", "rust_register_toolchains")

rules_rust_dependencies()

rust_register_toolchains()

