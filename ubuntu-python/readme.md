Basic up and running python container image with ubuntu as base

commands
1) docker build -t sapan2211/ubuntu-python:1.0 .
2) docker push sapan2211/ubuntu-python:1.0
3) docker run -it sapan2211/ubuntu-python:1.0
4) docker commit <ctr-id> sapan2211/ubuntu-python:2.0 #commit after some manual modifications in the container
