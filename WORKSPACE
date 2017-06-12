# nanopb
bind(
    name = "nanopb",
    actual = "//third_party/nanopb",
)

# Boringssl
bind(
    name = "libssl",
    actual = "@submodule_boringssl//:ssl",
)

new_local_repository(
    name = "submodule_boringssl",
    build_file = "third_party/boringssl-with-bazel/BUILD",
    path = "third_party/boringssl-with-bazel",
)

# Zlib
bind(
    name = "zlib",
    actual = "@submodule_zlib//:z",
)

local_repository(
    name = "submodule_zlib",
    path = "third_party/zlib",
)


# Protobuf
bind(
    name = "protobuf",
    actual = "@com_google_protobuf//:protobuf",
)

bind(
    name = "protobuf_clib",
    actual = "@com_google_protobuf//:protoc_lib",
)

bind(
    name = "protocol_compiler",
    actual = "@com_google_protobuf//:protoc",
)

new_local_repository(
    name = "com_google_protobuf",
    build_file = "third_party/protobuf/BUILD",
    path = "third_party/protobuf",
)

# grpc
bind(
    name = "bazel",
    actual = "@submodule_grpc//:bazel",
)

bind(
    name = "grpc++",
    actual = "@submodule_grpc//:grpc++",
)

bind(
    name = "grpc++_codegen_proto",
    actual = "@submodule_grpc//:grpc++_codegen_proto",
)

bind(
    name = "grpc_cpp_plugin",
    actual = "@submodule_grpc//:grpc_cpp_plugin",
)

git_repository(
    name = "submodule_grpc",
    remote = "https://github.com/grpc/grpc",
    tag = "v1.4.0-pre1",
)
