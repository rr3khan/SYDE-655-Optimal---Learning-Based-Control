# Reinforcement Learning Based Control Cart Pole  

## Description

Experiments to control the cart pole system using reinforcement learning algorithms. The cart pole system is a classic control problem in the field of control theory. The goal is to balance the pole on the cart by moving the cart left or right. The system is considered unstable because the pole will fall if it is not balanced.  

## Prerequisites

Before you begin, ensure you have met the following requirements:
- Docker is installed on your machine.
- Docker Desktop is installed if on Windows or Mac. 

## Installation

To set up the project environment, follow these steps:

1. Clone the repository 
2. Run the following command to build the Docker image:
```
    docker build -t <image-name> .
``` 

## Running the Docker Container

Run the Docker container with port 8888 mapped:

``` 
    docker run -p <local port>:8888 -it -v <local directory to mount>:<target directory>
``` 
Similarly this can be done using docker desktop

![Docker Desktop Port Mapping](docker_mapping_port_mapping.png "Docker Desktop Port Mapping")


## Accessing Jupyter Notebook

After running the container, you'll see an output in the terminal with a URL to access Jupyter Notebook. It will look something like this:

``` 
    http://127.0.0.1:8888/?token=your-token-here
``` 

Copy the URL and paste it into your web browser. Enter the token from the Docker terminal when prompted.