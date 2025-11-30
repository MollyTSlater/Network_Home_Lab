# Lab One: Learning Basics

1. **Identify Network Interfaces and IP Addresses**

```
sudo apt install net-tools
```
We want to install net-tools for this project in order to access ifconfig. Net-tools also contains other useful _, such as _.

```
ip a
```
This command displays all network interfaces and their associated IP addresses on our server. 

![Network_Interfaces_and_IP_Addresses](<Network_Interfaces_and_OP_Addresses.png>)

2. **Check Open Ports**

This command allows us to see all open ports, including listing which ones are listening.
```
sudo netstat -tuln
```

![Open_Ports](<Open_Ports.png>)

3. **Analyze Network Connections**

```
sudo lsof -i -P -n
```

![Network_Connections](<Network_Connections.png>)

4. Perform Network Scanning with Nmap

```
sudo nmap -sS -O localhost
```

![Network_Scanning](<Network_Scanning.png>)

5. **Check for Open Ports on the Server's Network**

```
sudo nmap -sP 192.168.1.0/24
```

![Open_Ports_on_Network](<Open_Ports_on_Network.png>)

6. **Check for Services and Versions**

```
sudo nmap -sV localhost
```
![Services_and_Versions](<Services_and_Versions.png>)

7. **Identify Potential Vulnerabilities**

```
sudo nmap --script vuln localhost
```
![Potential_Vulnerabilities](<Potential_Vulnerabilities.png>)

8. **Inspect Network Traffic**

```
sudo tcpdump -i eth0
```
![Network_Traffic](<Network_Traffic.png>)

9. Monitor Network Connections in Real-Time

```
sudo watch -n 1 netstat -tulnp
```
![Monitor_Network_Connections](<Monitor_Network_Connections.png>)

10. Check Firewall Rules

```
sudo ufw status verbose
```
![Firewall_Rules](<Firewall_Rules.png>)
