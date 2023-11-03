Part 1: Docker file Creation, GitHub and Docker Hub Integration.

Step 1: Using simple Hello World App in Python. Step 2: Installed Python
(Programming Language),FastAPI,Uvicorn (Libraries) as Dependencies for
this APP. Step 3: Docker file created. (File name dockerFile). Step 4:
Docker image created successfully as follows:
C:\\Users\\HP\\Desktop\\DockerLearning\>docker build -t helloworld-app .
\[+\] Building 24.4s (9/9) FINISHED docker:default =\> \[internal\] load
build definition from dockerfile 0.1s =\> =\> transferring dockerfile:
197B 0.0s =\> \[internal\] load .dockerignore 0.1s =\> =\> transferring
context: 2B 0.0s =\> \[internal\] load metadata for
docker.io/library/python:latest 0.0s =\> \[1/4\] FROM
docker.io/library/python:latest 0.2s =\> \[internal\] load build context
0.1s =\> =\> transferring context: 475B 0.0s =\> \[2/4\] COPY run.py
run.py 0.0s =\> \[3/4\] COPY Requirements.txt Requirements.txt 0.0s =\>
\[4/4\] RUN pip install -r Requirements.txt 23.7s =\> exporting to image
0.3s =\> =\> exporting layers 0.2s =\> =\> writing image
sha256:7da20d9f204c94a5ff5c7f09e5bf7116eecfc0cd5f433a04b8a9f71eeb8f1455
0.0s =\> =\> naming to docker.io/library/helloworld-app

Docker Image Created or build verified through docker images command.

REPOSITORY TAG IMAGE ID CREATED SIZE helloworld-app latest 7da20d9f204c
4 minutes ago 1.05GB

Docker Image running successcfully on localhost @ 2010 port

Step 5: To push the Docker image to Docker hub need to create the image
in a proper format as requireed by the docker hub run the following
command: docker tag helloworldpython haiderali956/helloworldapp:v1.0
Need to give username of docker hub and the name of the app in addition
to the tag or version of the app. Note: You need to provide the login
details for Dockerhub for the Pushing the image to dockerhub and run the
following command:

docker push haiderali956/helloworldapp:v1.0

And to pull the image use the following command: docker pull
haiderali956/helloworldapp:v1.0
