# nano

$ export DISPLAY=:0

$ xhost +

$ sudo docker run --net=host --runtime nvidia --rm --ipc=host -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v /tmp/argus_socket:/tmp/argus_socket --cap-add SYS_PTRACE -e DISPLAY=$DISPLAY -it nvcr.io/nvidia/l4t-ml:r32.6.1-py3

$ gst-launch-1.0 nvarguscamerasrc sensor_id=0 ! nvoverlaysink


#Mediapipe

https://github.com/PINTO0309/mediapipe-bin
