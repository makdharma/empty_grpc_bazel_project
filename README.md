# empty grpc bazel project
This repo has the preconfigured WORKSPACE and git submodules to get you started on using grpc with bazel.
To try this repo:
```
git clone https://github.com/makdharma/empty_grpc_bazel_project test
cd test
git submodule update --init
bazel build //examples/cpp/helloworld:*
```
This will build the ```greeter_client``` and ```greeter_server``` exacutables in ```bazel-bin/examples/cpp/helloworld``` subdirectory.
