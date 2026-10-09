#PART B -SSH

What is SSh?
SSH stand for Secure Shell.

It is how I connect to my EC2 Linux server from my laptop and actually control it.

Without SSH I cannot do anything on server.

WHY SSH IMPORTANT?

SSH is basically a tool that we use:
To log into the serve.
Run Linux commands.
Install things like Nginx.
Check services are running,and fix issues when something fails.

SSH uses TCP port 22

WHAT IS AUTHENTICATION ?

It is a process of checking that someone is allowed to access a system.

PASSWORD vs SSH Key Authentication

Password authentication require a user to enter a password
SSH key authentication uses a private key and a matching public key.

WHERE IS THE PRIVATE KEY STORED ?

I keep my private key (.pem file) on my laptop in asecure folder with permisions locked down.

WHY SHOULD I NEVER UPLOAD MY PRIVATE KEYS TO GITHUB

If I push my private key to github , anyone on the internet could find it and use it to log into my EC2 instance.
Security risk.

WHAT I LEARNED

I learned how important SSh is for managing cloud servers.
It is not about connecting,it's about doing it securely.
Understanding why we protect the private key.
Understanding why we restrict port 22 and how key-based login is safer than using a password.


