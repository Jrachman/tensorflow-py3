# tensorflow-py3-docker

**Steps to getting Jupyter running:**

 1. `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 julianrachman/tensorflow-py3:latest /bin/bash`
 2. `cd /`
 3. `./run_jupyter.sh`
 4. Navigate into the `notebooks` directory and you are set!
