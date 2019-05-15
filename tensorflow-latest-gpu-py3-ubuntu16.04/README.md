# Dockerfile
Tensorflow latest gpu on Ubuntu16.04 and Python3.5

# How to Install
docker build -t tensorflow-latest-gpu-py3

# How to Run
```
$ docker run --rm -it tensorflow-latest-gpu-py3  bash

________                               _______________                
___  __/__________________________________  ____/__  /________      __
__  /  _  _ \_  __ \_  ___/  __ \_  ___/_  /_   __  /_  __ \_ | /| / /
_  /   /  __/  / / /(__  )/ /_/ /  /   _  __/   _  / / /_/ /_ |/ |/ / 
/_/    \___//_/ /_//____/ \____//_/    /_/      /_/  \____/____/|__/


WARNING: You are running this container as root, which can cause new files in
mounted volumes to be created as the root user on your host machine.

To avoid this, run the container by specifying your user's userid:

$ docker run -u $(id -u):$(id -g) args...

root@7c3e291cc697:/# python --version
Python 3.5.2
root@7c3e291cc697:/# python3.
python3.5          python3.5-config   python3.5m         python3.5m-config  python3.7          python3.7m         
root@7c3e291cc697:/# python3.7 --version
Python 3.7.3
root@7c3e291cc697:/# python3.7 -c "import tensorflow as tf; print(tf.__version__)"
1.13.1
```
