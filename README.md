# set up
[Bazel install](http://bazel.io/docs/install.html)

# build

```
$ bazel build //:ios-app --ios_sdk_version=9.1 --ios_cpu="arm64" --default_ios_provisiong_profile=":bazelSample.mobileprovision"
```
