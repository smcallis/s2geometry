package(default_visibility = ["//visibility:public"])

cc_library(
    name = "bignum",
    srcs = ["bignum.cc"],
    hdrs = ["bignum.h"],
    visibility = ["//visibility:private"],
    deps = [
        "@abseil-cpp//absl/algorithm:container",
        "@abseil-cpp//absl/container:inlined_vector",
        "@abseil-cpp//absl/log:absl_check",
    ],
)

cc_library(
    name = "exactfloat",
    srcs = ["exactfloat.cc"],
    hdrs = ["exactfloat.h"],
    deps = [
        ":bignum",
        "//s2/base:logging",
        "//s2/base:port",
    ],
)

cc_test(
    name = "bignum_test",
    srcs = ["bignum_test.cc"],
    deps = [
        ":bignum",
        "@abseil-cpp//absl/random:bit_gen_ref",
        "@boringssl//:crypto",
        "@googletest//:gtest_main",
    ],
)
