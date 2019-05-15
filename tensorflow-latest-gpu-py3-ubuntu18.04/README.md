# Dockerfile
Tensorflow latest gpu on Ubuntu18.04 and Python3.6

# How to Install
$ docker build -t tensorflow-latest-gpu-py3-ubuntu18.04 .

# How to Run
```
$ docker run --rm -it tensorflow-latest-gpu-py3-ubuntu18.04 bash
root@3e2543f53871:/#
root@3e2543f53871:/# python3.6 -c "import tensorflow as tf; print(tf.__version__)"
1.13.1
root@3e2543f53871:/# nvidia-smi
Wed May 15 13:16:25 2019       
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 418.67       Driver Version: 418.67       CUDA Version: 10.1     |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|===============================+======================+======================|
|   0  GeForce GTX 1080    Off  | 00000000:01:00.0  On |                  N/A |
| 28%   56C    P2    37W / 200W |   7964MiB /  8119MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+
|   1  GeForce GTX 1080    Off  | 00000000:02:00.0 Off |                  N/A |
|  0%   41C    P8     6W / 200W |    117MiB /  8119MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+
                                                                               
+-----------------------------------------------------------------------------+
| Processes:                                                       GPU Memory |
|  GPU       PID   Type   Process name                             Usage      |
|=============================================================================|
+-----------------------------------------------------------------------------+
```
