# Container Observability

## Overview

In this activity, I learned how to run a web server inside a Docker container and test its response using HTTP requests. I used Nginx as the web server and Docker to run the application in the background.

## Running the Nginx Server

I created a Docker container named clientwebsite and assigned port 8080 to access the Nginx web server. After starting the container, I checked its status to make sure it was running properly.

## Testing Website Access

I used the curl command to send three requests to http://localhost:8080. The server responded with the default Nginx welcome page, which showed that the website was accessible and responding to requests.

## Testing an Invalid Page

I also tried opening /hidden-admin-page using curl. Since the page was not available on the website, Nginx returned a 404 Not Found response. This test helped me understand how a web server responds when a user requests a page that does not exist.

## Application Logging and Error Investigation

### Recorded 404 Error

text
172.17.0.1 - - [11/Oct/2026:11:15:49 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0"

### Why Application Logs Matter

Application logs help administrators understand how a web server behaves by recording incoming requests and their responses. When an error occurs, these records provide useful details that can help locate the problem and make it easier to fix.
