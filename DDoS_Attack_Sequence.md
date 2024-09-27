```mermaid
sequenceDiagram
actor Attacker
Note left of Attacker: An attacker is usally a<br/>hacktivist or a malicious actor
Note left of BotNet: A BotNet is a group of computers or <br/>IOT that have been hijacked and controlled<br/> by the attacker.
Attacker->>BotNet: The attacker will try to create a network  <br/>of botnets to perfrom the DDOS attack.a<br/>To create a botnet the attacker uses <br/>  Malware that can usually infect IOT devices
BotNet-->>Attacker: The botnet will respond to the bot-herder
participant BotNet
BotNet->>WebServer: Layer 7 DDOS: This attack is designed to target<br/>a website application layer in an attempt<br/>to overwhelm the server.
BotNet->>WebServer: HTTP Get: This attack will send a large<br/>amount of request to a webserver. Typically<br/>these request can include images, videos,<br/>or scripts. The excessive amount of request<br/>can exhuast the server and the end result<br/>is a DDOS attack.
BotNet->>WebServer: Slowloris: This attack consist of sending<br/>incomplete HTTP request. By sending these<br/>incomplete request the attacker is able to <br/>maintain connections open for along period<br/>of time and by doing this, the server will<br/>eventually reach its connection capacity.<br/>This attack will eventually use up resources.
participant WebServer
rect rgba(255,255,255) 
participant Firewall
Firewall-->>WebServer: A level 7 firewall can help against DDOS <br/>attacks on the application layer because<br/>it will analyze incoming traffic in depth<br/>to see if it contains any malware.
Firewall-->>WebServer: A level 7 firewall also has knowledge<br/>of HTTP and can detect malicious SQL
end
```
In the diagram above I have explained how a DDOS attacks works and the type of DDOS attack. According to the diagram it is a level 7 attack because it has "WebServer".
A level 7 DDOS attack on the webser are very common attacks. The attack usually starts by a hacktivist or an actor that must first create a BotNet, which will eventually flood a server
with multiple requests. To create a botnet the attacker will first try to infect multiple computers usually through malware such as a trojan. The goal of this attack is to infect as many
machines as possible. Once these machines are infected they will follow the command of the attacker who at this point is called a bot-herder. After the successful attacks on the IOT the
bot-herder will start the exploits. These bot-nets will attack the layer 7 because the layer seven is the application layer. One specific attack the bot-net uses is a HTTP GET, this will
send large amount of request to a server and usually it will request videos, images, or scripts. These request will cause the serves to become overwhelm and result in a DDOS attack.
Another attack is the slowrolis attack, this attack will send incomplete HTTP request and by doing this the connections maintain open for a long period of time and cause the server to 
to use up resources and exhaust the servers. This attack is very successful because of how slow the attack is and can maintain undetected.
