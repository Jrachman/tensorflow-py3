# tensorflow-py3-docker

**Pre-built image**

 There is a pre-built image that was created: https://hub.docker.com/r/julianrachman/tensorflow-py3/. 

 Use `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 julianrachman/tensorflow-py3:latest /bin/bash` to run this.

**Local build**

 Download this repository, extract, and navigate to the directory where the `Dockerfile` is located using your terminal.

 Then execute the command `docker build .`.
 
 After the build is complete, execute `docker images`, find the most recent `IMAGE ID`.
 
 Now execute `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 <IMAGE ID> /bin/bash`.
 
 **Docker Compose build**
 
 
