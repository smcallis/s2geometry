package(default_visibility = ["//visibility:public"])

cc_library(
    name = "exactfloat",
    srcs = ["exactfloat.cc"],
    hdrs = ["exactfloat.h", "bignum.h"],
    deps = [
        "//s2/base:port",
        "//s2/base:logging",
        "@abseil-cpp//absl/log:log",
        "@abseil-cpp//absl/log:absl_check",
        "@abseil-cpp//absl/strings:str_format",
        "@abseil-cpp//absl/container:inlined_vector",
        "@abseil-cpp//absl/numeric:bits",
        "@abseil-cpp//absl/numeric:int128",
        "@abseil-cpp//absl/strings:ascii",
    ],
)
