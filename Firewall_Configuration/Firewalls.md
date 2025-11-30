# Lab Two: Firewall

1. **Enable UFW (Uncomplicated Firewall)**

   Ensure the system is up to date using the commands:

   ```
   sudo apt update
   sudo apt upgrade -y
   ```

Question: If you are remotely accessing your server, why is it important to allow
traffic through port 22 before enabling UFW?
It is important because port 22 is the ssh port, and you may essentially "lock yourself out" of the server.

2. **Enable UFW Logging**

   
