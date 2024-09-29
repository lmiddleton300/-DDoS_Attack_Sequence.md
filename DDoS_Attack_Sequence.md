
```mermaid
sequenceDiagram
 participant Attacker
 participant BotNet
 participant WebServer
 participant Firewall
 
 Attacker->>BotNet: Malware installed onto endhost via emails and websites, without the user knowing
BotNet->>Attacker: established botnets now report to the the attacker
Attacker->>BotNet: attacker sends instructions on when to start DDoS attack
BotNet->>Server: DDoS attack starts
```
