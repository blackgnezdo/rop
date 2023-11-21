load("@rules_rust//rust:toolchain.bzl", "rust_toolchain")

rust_toolchain(
    name = "rust_openbsd_impl",
    binary_ext = "",
    dylib_ext = ".so",
    exec_triple = "x86_64-unknown-openbsd",
    rust_doc = "/usr/local/bin/rustdoc",
    rust_std = "/usr/local/bin/rust_std",
    rustc = "/usr/local/bin/rustc",
    rustc_lib = "/usr/local/bin/rustc_lib",
    staticlib_ext = ".a",
    stdlib_linkflags = ["-lpthread"],
    target_triple = "x86_64-unknown-openbsd",
)

toolchain(
    name = "rust_openbsd",
    exec_compatible_with = [
        "@platforms//cpu:x86_64",
        "@platforms//os:openbsd",
    ],
    target_compatible_with = [
        "@platforms//cpu:x86_64",
        "@platforms//os:openbsd",
    ],
    toolchain = ":rust_openbsd_impl",
    toolchain_type = "@rules_rust//rust:toolchain",
)
