# Lab Two: Firewall

1. **Enable UFW (Uncomplicated Firewall)**

   a. 
   Ensure the system is up to date using the commands:

   ```
   sudo ufw status
   ```

   b.
   ```
   sudo ufw allow 22/tcp
   ```

'Question: If you are remotely accessing your server, why is it important to allow
traffic through port 22 before enabling UFW?'
It is important because port 22 is the ssh port, and you may essentially "lock yourself out" of the server.

   c.
   ```
   sudo ss -tuln 
   ```

   d.
   ```
   sudo ufw enable
   ```

   e.
   ```
   sudo ufw status
   ```

   f.

   g.
   ```
   sudo ufw status verbose
   ```
   

2. **Enable UFW Logging**

   
