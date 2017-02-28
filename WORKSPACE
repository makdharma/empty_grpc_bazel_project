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
    actual = "@submodule_protobuf//:protobuf",
)

bind(
    name = "protobuf_clib",
    actual = "@submodule_protobuf//:protoc_lib",
)

bind(
    name = "protocol_compiler",
    actual = "@submodule_protobuf//:protoc",
)

new_local_repository(
    name = "submodule_protobuf",
    build_file = "third_party/protobuf/BUILD",
    path = "third_party/protobuf",
)

# grpc
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
    commit = "fa301e3674a1cc786eb4dd4253a0e677f2eb68e3", #v1.1.2
)
