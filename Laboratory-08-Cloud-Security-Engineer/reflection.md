# Laboratory 08 – Mission Reflection

This laboratory helped me understand the importance of server security. I learned that a host-based firewall protects a server by controlling incoming and outgoing connections. Even if attackers get past the network firewall, the server's own firewall can still block unwanted connections. This adds another layer of protection and helps keep the server safe.

Managing open network ports is also important because every open port can be a possible entry point for attackers. If unnecessary ports are open, attackers may find ways to access the server. In this activity, I allowed SSH and port 8080 because they were needed for server access and the web application. I also applied the Default Deny policy to block incoming connections that were not allowed.

In a real enterprise environment, leaving a database port like 3306 for MySQL open to the public internet is dangerous. Attackers may try to access the database, guess passwords, or take advantage of security weaknesses. If they gain access, they could steal, change, or delete important information. Database access should only be allowed from trusted servers or authorized networks.

Completing this mission changed my perspective on server security. Before, I thought that running a web server was enough to make an application work. Now, I understand that security settings are also important. Even a simple mistake, such as leaving an unnecessary port open, can create a security risk. Testing the application and checking firewall rules helped me see how small steps can improve protection.

With eight completed missions, my GitHub portfolio shows my progress in learning cloud computing. It contains my activities, commands, documentation, reflections, and screenshots of my work. I am proud of what I have completed because each mission helped me gain new skills. I know I still have more to learn, but I am becoming more confident in using Linux, Docker, and basic security tools. These experiences will help me prepare for future cloud computing tasks.
