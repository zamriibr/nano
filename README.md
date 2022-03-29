# nano

$ export DISPLAY=:0

$ xhost +

$ sudo docker run --net=host --runtime nvidia --rm --ipc=host -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v /tmp/argus_socket:/tmp/argus_socket --cap-add SYS_PTRACE -e DISPLAY=$DISPLAY -it nvcr.io/nvidia/l4t-ml:r32.6.1-py3

$ gst-launch-1.0 nvarguscamerasrc sensor_id=0 ! nvoverlaysink


#Mediapipe

$ python3 -m pip install mediapipe-python-aarch64/mediapipe-0.8.4-cp38-cp38-linux_aarch64.whl
$ sudo pip3 install mediapipe-0.8.5_cuda102-cp36-none-linux_aarch64.wh

https://github.com/PINTO0309/mediapipe-bin

sudo pip3 install opencv_contrib_python
git clone https://github.com/PINTO0309/mediapipe-bin
cd mediapipe-bin

sudo apt install curl

./v0.8.5/numpy119x/mediapipe-0.8.5_cuda102-cp36-cp36m-linux_aarch64_numpy119x_jetsonnano_L4T32.5.1_download.sh

sudo pip3 install numpy-1.19.4-cp36-none-manylinux2014_aarch64.whl
sudo pip3 install mediapipe-0.8.5_cuda102-cp36-none-linux_aarch64.whl
pip3 install dataclasses 
