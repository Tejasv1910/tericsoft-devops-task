\# Tericsoft DevOps Internship Task



A simple Dockerized web application deployed on an AWS EC2 instance using Ubuntu and Docker.



\## Project Overview



This project demonstrates how to containerize a basic web application using Docker and deploy it on an AWS EC2 virtual machine.



The application serves a static HTML page using Python's built-in HTTP server.



\## Technologies Used



\- AWS EC2

\- Ubuntu Server 24.04 LTS

\- Docker

\- Python 3.12

\- HTML



\## EC2 Instance Configuration



| Component | Configuration |

|---|---|

| Instance Type | t3.micro |

| vCPU | 2 |

| RAM | 1 GiB |

| Storage | 8 GiB gp3 |

| Operating System | Ubuntu 24.04 LTS |

| Application Port | 8081 |



The selected instance configuration is suitable for this lightweight demonstration application.



\## Run Locally with Docker



Build the Docker image:



```bash

docker build -t tericsoft-web:1.0 .

```



Run the container:



```bash

docker run -d --name tericsoft-web -p 8081:8081 tericsoft-web:1.0

```



Open the application:



```text

http://localhost:8081

```



\## Deployment



The Docker container is deployed on AWS EC2 and the application is accessible through port `8081`.



\## Project Files



\- `index.html` – Application webpage.

\- `Dockerfile` – Instructions to build the Docker image.

