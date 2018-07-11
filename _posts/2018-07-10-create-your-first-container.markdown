---
layout: post
title:  "Create your first container"
date:   2018-07-10 22:32:48 -0700
categories: post
---

### Learn how to create a container using Docker

Install Docker

Create a Dockerfile cat Dockerfile FROM ubuntu:latest RUN apt-get update -y

Create an image using Docker file docker build -t new_image .

docker image ls

Creating a container docker run -it new_image /bin/bash
