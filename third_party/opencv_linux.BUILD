# taken from setup instructions for opencv 4 at
# https://google.github.io/mediapipe/getting_started/install.html#installing-on-debian-and-ubuntu

package(default_visibility = ["//visibility:public"])

licenses(["notice"])  # BSD license

exports_files(["LICENSE"])

cc_library(
  name = "opencv",
  hdrs = glob([
    "include/opencv4/opencv2/**/*.h*",
  ]),
  includes = [
    "include/opencv4/",
  ],
  linkopts = [
    "-L/usr/local/lib",
    "-l:libopencv_core.so",
    "-l:libopencv_calib3d.so",
    "-l:libopencv_features2d.so",
    "-l:libopencv_highgui.so",
    "-l:libopencv_imgcodecs.so",
    "-l:libopencv_imgproc.so",
    "-l:libopencv_video.so",
    "-l:libopencv_videoio.so",
  ],
)
