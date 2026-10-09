# Linux Foundation

What I Learned In this lab, I learned how linux users,processes,services,ports,and networks all work together om my AWS EC2 instance.

1. USER 
Command: whoami
Result: ec2-user

This showed me which user I was currently logged in as on server.

2. PROCESS
Command:ps aux

When I ran this, I could see lots of processes running under dufferent users, including root and ec2-user.
It helped me to understand that a process is just a program that is actively running on the Linux server.

3. SERVICE
Command:systemctl status ssd
Result:active(running)

This confirmed that the ssh service was running properly on my EC2 instance.

4. PORT
Commnd:sudo ss -tuipn | grep:22
Result: TCP: port22,
        Process:sshd
        PID:1884

This proved that the ssh service is listening on port 22 for incoming network connections.

5. NETWORK
Command:ip -4 addr show
Result inerface:ens5
       private IP:10.0.3.109
       subnet:20
This showed me that my EC2 network interface is active and connected.

# Conclusion

Through this lab I now have a clearer picture of:

How Linux user interacts with processes and services,
How services use ports to communicate over the network,
And how to troubleshoot SSH by checking it's service status,process ID,port,and network configaration.
