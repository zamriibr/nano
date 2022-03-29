# nano

$ export DISPLAY=:0
$ xhost +
$ sudo docker run -it --rm --net=host --runtime nvidia  -e DISPLAY=$DISPLAY -v /tmp/.X11-unix/:/tmp/.X11-unix nvcr.io/nvidia/l4t-ml:r32.6.1-py3

$ gst-launch-1.0 nvarguscamerasrc sensor_id=0 ! nvoverlaysink

$ gst-launch-1.0 -v -e videotestsrc is-live=1 num-buffers=250 ! video/x-raw, format=\(string\)NV12, framerate=\(fraction\)25/1 ! nvvidconv ! nvv4l2h264enc ! h264parse ! matroskamux ! filesink location=test.mkv
