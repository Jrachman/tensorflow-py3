# tensorflow-py3-docker

Designed for heavy computations in TensorFlow using Python 3.

**Dockerfile:** https://github.com/Jrachman/tensorflow-py3-docker/blob/master/Dockerfile

**Developer:** Julian Rachman (jmrachman@gmail.com)

---

**Setup and run**

*Pre-built image*

1. There is a pre-built image that was created: https://hub.docker.com/r/julianrachman/tensorflow-py3/

2. Execute `docker pull julianrachman/tensorflow-py3:latest` in the terminal.

3. Use `docker run -it --network=host -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 julianrachman/tensorflow-py3:latest` to run this.

4. Run `config/run_jupyter.sh --allow-root` and you are set! Just visit http://localhost:8888 and the password should be "pass."

*Local build*

1. Download the GitHub repository (https://github.com/Jrachman/tensorflow-py3-docker/), extract, and navigate to the directory where the `Dockerfile` is located using your terminal.

2. Then execute the command `docker build .`
 
3. After the build is complete, execute `docker images`, find the most recent `IMAGE ID`
 
4. Now execute `docker run -it -p 8888:8888 -e "PASSWORD=pass" --name jrtfpy3 <IMAGE ID>`

4. Run `config/run_jupyter.sh --allow-root` and you are set! Just visit http://localhost:8888 and the password should be "pass."
 
*Docker Compose build*
 
1. `docker-compose build`
 
2. `docker-compose up`

---

**Git**

*Clone*

1. Navigate to the Docker container terminal and make sure you are in the "notebooks" directory. 

2. `git clone <your repsoitory URL>`

*Initial push*

1. Navigate to the Docker container terminal and make sure you are in the "notebooks" directory. 

2. Configure Git for the first time by running the command `git config --global user.name "<NAME>" && git config --global user.email "<EMAIL>"`

3. `git init`

4. `git add .`

5. `git commit -m "First commit"`

6. `git remote add origin <remote repository URL>`

7. `git remote -v`

8. `git push -u origin master`

*Further pushing*

1. Navigate to the Docker container terminal and make sure you are in the "notebooks" directory. 

2. `git status`

3. `git add .` 

4. `git commit -m "<MESSAGE>"`

5. `git push -u origin master`

 
