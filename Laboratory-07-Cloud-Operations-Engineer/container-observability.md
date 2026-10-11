# Container Observability Report

## Introduction

This laboratory activity focused on running and monitoring a web server inside a Docker container. I used Nginx to test website accessibility, generate HTTP requests, examine server logs, and check the resources used by the application.

## 1. Deploying the Web Server

I started an Nginx container using Docker and named it clientwebsite. I used port mapping to make the website accessible through port 8080 on the host machine.

The command I executed was:

docker run -d --name clientwebsite -p 8080:80 nginx

After running the command, I checked the container status to confirm that the web server was running.

## 2. Testing Website Requests

I used the curl command to access http://localhost:8080 three times. The web server returned the default Nginx welcome page for all three requests, indicating that the website was accessible and responding properly.

To test how the server handles an unavailable page, I ran:

curl http://localhost:8080/hidden-admin-page

The request returned a *404 Not Found* response because the requested page was not available on the server.

## 3. Checking Application Logs

Application logs provide a record of requests received by the web server. I retrieved the logs using the following command:

docker logs clientwebsite

### Recorded Error

The following line shows the failed request from my terminal:

text
172.17.0.1 - - [11/Oct/2026:11:15:49 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"

### Why Logs Are Important

Logs help administrators track website activity and identify requests that result in errors. By reviewing these records, they can investigate problems more easily and determine what needs to be corrected.

## 4. Monitoring Container Resources

I used the docker stats command to view the resource consumption of the running Nginx container. This tool displayed information about CPU usage, memory consumption, network traffic, and disk input/output.

### Recorded Docker Statistics

| Metric | Recorded Value |
|---|---|
| Container Name | clientwebsite |
| CPU Usage | 0.00% |
| Memory Usage | 2.793 MiB |
| Memory Limit | 1.859 GiB |
| Memory Usage Percentage | 0.15% |
| Network I/O | 4.58 kB / 6.89 kB |
| Block I/O | 49.2 kB / 12.3 kB |
| PIDs | 2 |

### Results and Observation

At the time of the screenshot, the container used 0.00% CPU and 2.793 MiB of memory. These results show low resource consumption during the observation period, but additional monitoring would be needed to determine how the container performs under heavier traffic.
