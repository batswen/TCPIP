# Netzwerkgrundlagen

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
##### Merksätze
(Englisch, 1 bis 7) Please Do Not Throw Salami Pizza Away<br/>
(Deutsch, 7 bis 1) Alle deutschen Studenten trinken verschiedene Sorten Bier
### BEzeichnungen
Name (Langform) [Port]<br/>
MAC (Media-Access-Control)<br/>
IP (Internet Protocol)<br/>
TCP (Transport Control Protocol)<br/>
UDP (User Datagram Protocol)<br/>
DNS (Domain Name Service) [53]<br/>
LDAP (Lightweight Directory Access Protocol) [TCP/UDP]<br/>
DHCP (Dynamic Host Configuration Protocol) [67 Server/Relay agent, 68 Client]<br/>
HTTP (HyperText Transfer Protocol) [80]<br/>
HTTPS (HyperText Transfer Protocol Secure) [443]
### IP-Adressen (IPv4)
IPv4-Adressen bestehen aus vier vorzeichenlosen Bytes, Oktett genannt, getrennt durch je einen Punkt.<br/>
```
Beispiel: 192.168.0.1
Beispiel: 200.200.200.200
```
#### Subnetzmaske
Die Subnetzmaske unterteilt die IP-Adresse in Netzwerkteil und Hostteil. Der Netzwerkteil wird durch Einsen (links) angezeigt, der Hostteil (rechts) durch Nullen. Nach der ersten Null kann keine Eins mehr vorkommen.</br>
Beispiel: 255.255.255.0 (Binär: 11111111.11111111.11111111.00000000)<br/>
Beispiel: 255.255.192.0 (Binär: 11111111.11111111.11000000.00000000)<br/>
Als Kurzform der Subnetzmaske hat sich der Suffix etabliert, hierbei wird lediglich die Anzahl der Einsen angegeben. Der Suffix wird an die IP-Adresse angehängt.<br/>
```
Beispiel: 192.168.0.1/24 (für 255.255.255.0)
Beispiel: 192.168.0.1/20 (für 255.255.240.0)
Beispiel: 192.168.0.1/16 (für 255.255.0.0)
```
#### Gateway
Ein Gateway ist die Verbindung zwischen zwei Netzwerken.
#### Netzklassen
Der verfügbare 32-Bit-Adressbereich ist in fünf sog. Netzklassen unterteilt. Die Klassen A, B, C sind zur freien Verwendung gedacht, D ist für Multicasts gedacht und E ist für zukünftige Erweiterung reserviert. Aufgrund des IP-Adressmangels wurde Klasse E freigegeben.
```
Netzklasse Präfix Bereich                      Netzmaske
 A          0...     0.0.0.0 - 127.255.255.255  255.0.0.0
 B          10..   128.0.0.0 - 191.255.255.255  255.255.0.0
 C          110.   192.0.0.0 - 223.255.255.255  255.255.255.0
 D          1110   224.0.0.0 - 239.255.255.255
 E          1111   240.0.0.0 - 255.255.255.255
```
#### Subnetze
Über die Subnetzmaske kann ein Netzwerk in mehrere, von einander unabhängige Netzwerke unterteilt werden.
### IP-Adressen (IPv6)
