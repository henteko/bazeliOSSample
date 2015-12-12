objc_library(
  name = "BazelSampleClasses",
  srcs = [
    "bazelSample/AppDelegate.m",
    "bazelSample/ViewController.m",
  ],
  hdrs = glob(["bazelSample/*.h"]),
  storyboards = ["bazelSample/Base.lproj/LaunchScreen.storyboard", "bazelSample/Base.lproj/Main.storyboard"],
)

objc_binary(
  name = "ios-app-binary",
  srcs = [
    "bazelSample/main.m",
  ],
  deps = [
    ":BazelSampleClasses",
  ],
)

ios_application(
  name = "ios-app",
  binary = ":ios-app-binary",
  bundle_id = "com.henteko07.bazelSample",
  infoplist = "bazelSample/Info.plist",
  provisioning_profile = "bazelSample.mobileprovision",
)
