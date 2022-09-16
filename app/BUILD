android_library(
    name = "basic_lib",
    custom_package = "com.example.mediapipe.helloworld",
    srcs = ["java/com/example/mediapipe/helloworld/MainActivity.java"],
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
    deps = [
        "//third_party:androidx_constraint_layout",
        "//third_party:androidx_appcompat",
    ],
)

android_binary(
    name = "helloworld",
    custom_package = "com.example.mediapipe.helloworld",
    manifest = "AndroidManifest.xml",
    manifest_values = {
        "appName": "MediaPipe Hello World",
        "mainActivity": ".MainActivity",
    },
    multidex = "native",
    deps = [
        ":basic_lib",
    ],
)