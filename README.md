# STANDARD-ACL
STANDARD ACCESS CONTROL LIST
# Definition
A Standard ACL is a type of access control list used in Cisco networks to permit or deny traffic based solely on the source IP address of packets. It does not filter based on destination IP, port numbers, or protocols. Standard ACLs are primarily used to control network access and manage traffic flow at a basic level.
# Project Definition
A standard ACL was configured to control ICMP traffic between two LAN networks (192.168.0.0/24 and 192.168.1.0/24) interconnected via the 192.168.2.0/24 network. The ACL was applied to permit only specific devices to send ICMP packets, restricting unauthorized ping access across the network.

# STANDARD-ACL CLI-COMMANDS

Router# config terminal

Router(config)# ip access - list standard 10

Router(config - std - nacl )# permit 192.168.0.2 0.0.0.0

Router(config - std - nacl )# deny 192.168.0.3 0.0.0.0

exit

Router(config)# int gig 0/0/0

Router(config - if # ip access - group 10 out
