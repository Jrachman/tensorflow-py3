# tensorflow-py3-docker

**Pre-built image**

1. There is a pre-built image that was created: https://hub.docker.com/r/julianrachman/tensorflow-py3/. 

2. Execute `docker pull julianrachman/tensorflow-py3:latest` in the terminal.

2. Use `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 julianrachman/tensorflow-py3:latest /bin/bash` to run this.

**Local build**

1. Download this repository, extract, and navigate to the directory where the `Dockerfile` is located using your terminal.

2. Then execute the command `docker build .`.
 
3. After the build is complete, execute `docker images`, find the most recent `IMAGE ID`.
 
4. Now execute `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 <IMAGE ID> /bin/bash`.
 
**Docker Compose build**
 
1. `docker-compose build`
 
2. `docker-compose up`
 
