# Laboratory 08 – Mission Reflection

In this laboratory, I learned how to protect a server using a host-based firewall. A host-based firewall helps protect a server by blocking unwanted connections. Even if attackers get past the main network firewall, the server's own firewall can still help stop them. In my activity, I used UFW to control which connections were allowed.

Managing open network ports is important because open ports can be entry points for attackers. The more unnecessary ports a server has open, the more chances attackers have to find a weakness. In my activity, I allowed SSH and TCP port 8080 because they were needed for server access and my Nginx web application. I also used the Default Deny policy to block incoming connections by default.

In a real company, leaving MySQL port 3306 open to the public internet is dangerous. Attackers may try to log in and access important data. They could steal, change, or delete information if they succeed. That is why database ports should only be accessible to trusted servers or authorized users.

This mission changed how I think about server security. Before, I focused more on making the web server work. After running my Nginx container using Docker, setting up UFW, allowing the needed ports, and testing the application with `curl`, I understood that a working server also needs protection. I also checked the firewall status and rules to make sure my settings were applied.

With eight completed missions, my GitHub portfolio shows the work I have done and the skills I have learned in cloud computing. It includes my commands, documentation, reflections, and screenshots. I feel happy with my progress because I am learning how to use Linux commands, Docker, and basic security tools. I know I still have more to learn, but these activities help me become more confident and prepare for future cloud computing tasks.
