load("//bazel:build.bzl", "redpanda_cc_library")

redpanda_cc_library(
    name = "cloud_storage_clients",
    srcs = [
        "abs_client.cc",
        "abs_error.cc",
        "client_pool.cc",
        "client_probe.cc",
        "configuration.cc",
        "s3_client.cc",
        "s3_error.cc",
        "util.cc",
        "xml_sax_parser.cc",
    ],
    hdrs = [
        "abs_client.h",
        "abs_error.h",
        "client.h",
        "client_pool.h",
        "client_probe.h",
        "configuration.h",
        "logger.h",
        "s3_client.h",
        "s3_error.h",
        "types.h",
        "util.h",
        "xml_sax_parser.h",
    ],
    include_prefix = "cloud_storage_clients",
    visibility = ["//visibility:public"],
    deps = [
        "//src/v/base",
        "//src/v/bytes",
        "//src/v/bytes:iobuf",
        "//src/v/bytes:iostream",
        "//src/v/bytes:streambuf",
        "//src/v/cloud_roles",
        "//src/v/cloud_roles:types",
        "//src/v/config",
        "//src/v/container:intrusive",
        "//src/v/hashing:secure",
        "//src/v/http",
        "//src/v/json",
        "//src/v/metrics",
        "//src/v/model",
        "//src/v/net",
        "//src/v/ssx:future_util",
        "//src/v/ssx:sformat",
        "//src/v/strings:string_switch",
        "//src/v/thirdparty/libxml2",
        "//src/v/utils:base64",
        "//src/v/utils:functional",
        "//src/v/utils:log_hist",
        "//src/v/utils:named_type",
        "//src/v/utils:retry_chain_node",
        "//src/v/utils:stop_signal",
        "@boost//:beast",
        "@boost//:lexical_cast",
        "@boost//:property_tree",
        "@seastar",
    ],
)
