# Mission Reflection

This laboratory activity helped me understand the difference between using a Virtual Machine and using Docker containers. In a Virtual Machine, installing and starting an operating system usually takes more time because the VM needs its own operating system, virtual hardware, storage, and other resources. In Docker, a container can start much faster because it shares the host operating system kernel. In our activity, I was able to pull the Nginx image and run the container using only a few Docker commands.

The port mapping `-p 8080:80` was necessary because the Nginx web server was running inside the container on port 80. Port 8080 on the host was connected to port 80 inside the container. Because of this mapping, I was able to access and test the Nginx server using `curl http://localhost:8080`. Without port mapping, the web server inside the container would not be easily accessible from the host.

When I used `docker rm nginx-server`, the stopped container was removed. Any data stored only inside the container's writable layer can be lost when the container is removed. This showed me that containers should not be treated as permanent storage and that important data should be stored using volumes or other persistent storage.

I also learned how containerization can improve DevOps teamwork. Developers can package applications with their needed environment, while IT operations teams can run the same container consistently in different environments. This can reduce problems caused by differences in setup and make deployment faster.

My GitHub portfolio is also evolving because I am now adding more organized documentation, Docker commands, screenshots, and reflections. Compared with my earlier laboratory work, my portfolio now shows not only the results but also the process and skills I learned. It is becoming a better record of my cloud computing activities and progress.
