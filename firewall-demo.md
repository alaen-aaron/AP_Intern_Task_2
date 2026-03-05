# Firewall Demonstration

## Objective
Demonstrate how firewall rules can block network access.

## Blocking Port 80

Command used:

sudo iptables -A INPUT -p tcp --dport 80 -j DROP

## Testing with Nmap

Command:

nmap -p 80 192.168.56.104

Result:
The port appeared as filtered, indicating that the firewall successfully blocked access.

## Removing Firewall Rule

Command:

sudo iptables -F

## Conclusion
Firewall rules can effectively prevent unauthorized access and protect services from scanning or exploitation.
