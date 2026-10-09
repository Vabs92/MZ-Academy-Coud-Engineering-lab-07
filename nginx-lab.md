# Deploying Nginx on EC2
 
What is Nginx?
Nginx is a web server that is used to host websites and make them accessible over a network.

My Lab Environment
For this lab, I used an AWS EC2 instance running Amazon Linux 2023.

What I Did:

Checked if Nginx was installed.
Confirmed that the Nginx service was running.
Checked if Nginx is set to start automatically on boot.
Located the Nginx configuration file.Located the website files.
Checked if port 80 was listening.
Tested the website using my EC2 public IP address.

Commands I Used

rpm -q nginx
systemctl status nginx
systemctl is-enabled nginx
ls -l /etc/nginx/nginx.conf
ls -l /usr/share/nginx/html
sudo ss -tulpn | grep :80

My Test Results

Nginx was already installed.
The service was active and running.
Nginx was enabled to start automatically.
It was listening on TCP port 80.
When I opened the public IP in my browser, I saw the "Welcome to nginx!" page.

What I Learned

I learned how to check if a web server is installed, 
How to confirm that its service is running,
Where to find its configuration and website files,
And how to test if the website is actually accessible from a browser.
