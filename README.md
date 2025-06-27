# Task-4-Setup-and-Use-a-Firewall-on-Windows-Linux

 Linux Firewall Setup using UFW

## Objectives
- Understand and apply basic firewall rules
- Practice port blocking and allowing traffic
- Demonstrate traffic filtering with screenshots

## Commands Used
- `ufw status`, `ufw enable`, `ufw deny`, `ufw allow`, `ufw delete`
- Tested port blocking using `telnet`

🔧 Step-by-Step Commands with Explanation & Screenshots
1. Check UFW Status

sudo ufw status verbose
📸 Screenshot shows initial status: Status: inactive

2. Enable UFW

sudo ufw enable
📸 Screenshot shows UFW is now active

3. List Existing Rules

sudo ufw status numbered
📸 Screenshot of empty or default rules list

4. Block Inbound Traffic on Port 23 (Telnet)

sudo ufw deny 23
📸 Screenshot confirms rule added

5. Test Blocked Port (Example: telnet test locally or simulate with netcat)

telnet localhost 23
📸 Screenshot shows connection refused or blocked

6. Allow SSH (Port 22)

sudo ufw allow 22
📸 Screenshot shows SSH allowed

7. Remove Port 23 Block Rule

sudo ufw delete deny 23
📸 Screenshot confirms rule removed


## Outcome
- Gained hands-on experience in using UFW on Linux.
- Understood how firewalls filter inbound/outbound traffic based on rules.

## Screenshots
(Screenshots are included in the `/screenshots` folder)
