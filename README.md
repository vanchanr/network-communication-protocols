# network-communication-protocols

## Firewall
- we may need to allow access to internet in the firewall configurtion for our network programs

## Internet Protocol (IP)
- IPv4 (32 bit addresses) and IPv6 (128 bit addresses)

## IP Protocol Suite (TCP and UDP)
### TCP
- TCP (Transmission Control Protocol) is a connection-based protocol that provides a reliable flow of data between two computers in sequence
- used in HTTP, FTP, Telnet etc.

### UDP
- UDP (User Datagram Protocol) is a protocol that sends independent packets of data, called datagrams, from one computer to another with no guarantees about arrival in sequence
- UDP is not connection-based like TCP
- used in DNS, DHCP, ping, voice and video streaming etc.

## IP Addresses reserved for local networks
- **10.0.0.0** to **10.255.255.255**
- **172.16.0.0** to **172.31.255.255**
- **192.168.0.0** to **192.168.255.255**

## Subnet Mask
- expressed as **192.168.0.0/16**
- helps routers to determine which packets are local and which need to be forwarded to the network

## Loopback Address
- represents the local computer
- IPv4 - **127.0.0.1**
- IPv6 - **::1**

## Port
- tied with a specific process / application running on a computer
- to communicate over a network, you must know both the IP address and the port
- port numbers are 16 bits wide
- 1 to 1023: system ports
- 1024 to 49151: registered ports by IANA
- 49152 to 65535: dynamic, private or ephemeral
```
$ cat /etc/services
lists ports assigned to network services.some support TCP, some support UDP and some support both

$ cat /etc/hosts

$ ip addr show
```