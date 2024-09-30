
```mermaid
sequenceDiagram
 participant Attacker
 participant BotNet
 participant Firewall
 participant WebServer
 
 Attacker->>BotNet: Malware installed onto endhost via emails and websites, without the user knowing
BotNet->>Attacker: established botnets now report to the the attacker
Attacker->>BotNet: attacker sends instructions on when to start DDoS attack
Attacker->>Firewall: traffic to the webserver through the firewall is permitted
Attacker->>BotNet: Attacker triggers the DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
BotNet->>WebServer: DDoS attack
WebServer->>Firewall: informs the firewall about the high cpu usage and high bandwidth use
Firewall->>BotNet: Deep inspection of packets along with low bandwidth availability causes firewall to block ports and ip addresses. 
```
