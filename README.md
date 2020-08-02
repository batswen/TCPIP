# Netzwerke

### Das OSI-Schichtenmodell
#### Schicht 1
Bitübertragungsschicht / Physical layer<br/>
Hardware, z. B. Token ring, 1000 BASE-T
#### Schicht 2
Sicherungsschicht / Data link layer<br/>
Ethernet, WLAN, MAC, Token ring
#### Schicht 3
Vermittlungsschicht / Network layer<br/>
IP, IPsec, ICMP, IGMP
#### Schicht 4
Transportschicht / Transport layer<br/>
TCP, UDP
#### Schicht 5
Sitzungsschicht / Session layer<br/>
#### Schicht 6
Darstellungsschicht / Presentation layer<br/>
#### Schicht 7
Anwendungsschicht / Application layer<br/>
### Protokolle
3 IP<br/>
4 TCP UDP<br/>
Name (Langform) [Port]<br/>
DNS (Domain Name Service) [53]<br/>
LDAP (Lightweight Directory Access Protocol) [TCP/UDP]<br/>
DHCP (Dynamic Host Configuration Protocol) [67 Server/Relay agent, 68 Client]<br/>
### IP-Adressen (IPv4)
IPv4-Adressen bestehen aus vier vorzeichenlosen Bytes, Oktett genannt, getrennt durch je einen Punkt.
Beispiel: 192.168.0.1
#### Subnetzmaske
#### Gateway
#### Netzklassen
```
Netzklasse Präfix Bereich Netzmaske
A           0...   0.0.0.0 - 127.255.255.255
B           10..   128.0.0.0 - 191.255.255.255
C           110.   192.0.0.0 - 223.255.255.255
D           1110   224.0.0.0 - 239.255.255.255
E           1111   240.0.0.0 - 255.255.255.255
```
#### Subnetze
### IP-Adressen (IPv6)
