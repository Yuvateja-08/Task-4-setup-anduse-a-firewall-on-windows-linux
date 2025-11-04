sudo apt install ufw -y
(Installs the UFW firewall package on your Linux system automatically, with -y to approve installation without manual confirmation.​)
sudo ufw enable
(Activates the UFW firewall, enforcing any defined rules and enabling packet filtering on system startup.​)
sudo ufw status verbose
(Displays the current status of the firewall, including whether it is active, its rule set, logging options, and default policies for incoming/outgoing traffic.​)
sudo ufw deny 23/tcp
(Blocks all incoming TCP connections on port 23 (Telnet), preventing unwanted or insecure remote access).​
sudo ufw deny 23
(Denies all traffic for port 23 regardless of protocol (TCP or UDP), adding further restrictions to Telnet access).​
sudo ufw allow 22
(Permits incoming connections on port 22 (typically used for SSH), ensuring you can remotely manage your system).​
sudo ufw status numbered
(Lists all current firewall rules with assigned numbers, making it easier to manage or delete rules later by referencing their position in the list).​

##Usage Purpose
These commands are commonly used during initial server setup, especially to:
Harden security by denying unused or risky ports such as Telnet (port 23).
Ensure remote management access over SSH (port 22) is allowed.
Check and verify firewall configuration in verbose detail.
Allow rule-based operations by number for improved manageability.
