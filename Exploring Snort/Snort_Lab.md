# Lab Three: Exploring Snort

1. **Update the System**

   Ensure the system is up to date using the commands:

   ```
   sudo apt update
   sudo apt upgrade -y
   ```

2. **Install Snort**

   Next install snort using the command:

   ```
   sudo apt install snort -y
   ```
   When doing so, be sure to choose a proper Network Interface, for me this was ens33. Also be sure to define your home network under HOME_NET.
   Use the command below to find the necessary confirguration info if needed:
   ```
   ip a
   ```
   
3: **Configure Snort**

   We can now configure out snort.conf file, using the command below:
   ```
   sudo nano /etc/snort/snort.conf
   ```
   Be sure to confirm that the HOME_NET section matches your network setup.

Step 4: Update and Manage Snort Rules

   If needed, community rules can be downloaded using:
   ```
   sudo wget https://www.snort.org/downloads/community/community-rules.tar.gz
   sudo tar -xvzf community-rules.tar.gz
   sudo cp community-rules/* /etc/snort/rules/
   ```
NEED TO
Check out the various rule files file in the rules directory. Which rules stick out to you? What is
the purpose of rules in general?


Step 5: Test Snort Configuration
![](<>)

Step 6: Running Snort in IDS Mode
![](<>)

Step 7: Viewing Snort Logs
Snort logs alerts in the /var/log/snort/ directory. Go to this directory. What files did you find here? 

Do any of them contain any content? Why or why not?

![](<>)

Step 8: Running Snort as a Daemon
![](<>)

