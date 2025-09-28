package(default_visibility = ["//visibility:public"])

cc_library(
    name = "bignum"
    srcs = ["bignum.cc"]
    hdrs = ["bignum.h"]
)

cc_library(
    name = "exactfloat",
    srcs = ["exactfloat.cc"],
    hdrs = ["exactfloat.h"],
    deps = [
        ":bignum",
        "//s2/base:types",
        "//s2/base:port",
        "//s2/base:logging",
        "@abseil-cpp//absl/container:inlined_vector",
        "@abseil-cpp//absl/log:absl_check",
        "@abseil-cpp//absl/log:log",
        "@abseil-cpp//absl/numeric:bits",
        "@abseil-cpp//absl/numeric:int128",
        "@abseil-cpp//absl/random:random",
        "@abseil-cpp//absl/strings:ascii",
        "@abseil-cpp//absl/strings:str_cat",
        "@abseil-cpp//absl/strings:str_format",
    ],
)
