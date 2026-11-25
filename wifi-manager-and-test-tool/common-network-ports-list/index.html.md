# Common Network Ports List and What They Mean

> A list of common TCP ports on home networks, what each service does, and how to check which ports a device has open on your own network.

- Web: https://apps.schimpf.es/wifi-manager-and-test-tool/common-network-ports-list/
- App: WiFi Scanner & Network Tools, https://apps.schimpf.es/wifi-manager-and-test-tool/index.md
A port is a number that tells a device which service a network connection is for. When you scan a device, an open port means a service is listening there. This page lists ports often seen on home and small office networks and explains how to read a scan.

Port names and numbers come from the IANA Service Name and Transport Protocol Port Number Registry. Some ports in the list below, such as 5000 and 9100, are used by convention more than by registration.

## Common ports

| Port | Service | What it is |
|---|---|---|
| 21 | FTP | File transfer. Unencrypted. |
| 22 | SSH | Encrypted remote login and file copy. |
| 23 | Telnet | Old remote login. Unencrypted. |
| 25 | SMTP | Sending email between servers. |
| 53 | DNS | Name lookups. Routers often answer here. |
| 80 | HTTP | Web pages, including many router and camera admin pages. |
| 110 | POP3 | Fetching email. Unencrypted. |
| 139 | NetBIOS | Windows name and file sharing, older. |
| 143 | IMAP | Fetching email. Unencrypted. |
| 443 | HTTPS | Encrypted web pages. |
| 445 | SMB | Windows and Samba file sharing. |
| 554 | RTSP | Video streams from IP cameras. |
| 631 | IPP | Network printing. |
| 993 | IMAPS | IMAP over TLS. |
| 995 | POP3S | POP3 over TLS. |
| 1883 | MQTT | Messages between smart home devices. |
| 3306 | MySQL | MySQL database. |
| 3389 | RDP | Windows Remote Desktop. |
| 5000 | UPnP | Used by some routers and NAS devices. |
| 5353 | mDNS | Local name discovery (Bonjour). |
| 8000, 8008, 8080, 8888 | HTTP alternate | Web pages on a second port. |
| 8443 | HTTPS alternate | Encrypted web pages on a second port. |
| 9100 | Printer | Raw printing to many network printers. |

Port numbers run from 1 to 65535. Ports 1 to 1023 are called well-known ports.

## How to read the result

- Open. A service answered the connection.
- Closed or filtered. Nothing answered, or a firewall dropped it. A scan cannot always tell these apart.
- Most open ports are fine. A printer on 631 or 9100 and a camera on 554 are expected.
- Look for unexpected ports. Telnet (23) open on a router or camera is a reason to check settings or update firmware. So is SMB (445) on a device that should not share files.
- Forward a port to the internet only if you know why. If you did not set it up, it should not be reachable from outside.

### Worked example

You scan a smart plug and a NAS on the same network.

1. The plug shows 80 open. Its app uses a small web page, so this is normal.
2. The NAS shows 22, 80, 443 and 445 open: SSH, web admin and file sharing. This is normal for a NAS.
3. The NAS also shows 23 open. Telnet is rarely needed. Turn it off in the NAS settings, then scan again to confirm it is closed.

## How a TCP connect scan works

The scanner tries to open a normal TCP connection to each port. If the connection succeeds, the port is open. It does not send harmful traffic, but it is visible to the device and to any firewall in between. This is why you should scan only your own network and devices you are allowed to test. Scanning someone else's network can be illegal where you live.

## Scan your own network with the app

The Tools screen in WiFi Scanner & Network Tools has a port scan with three presets and your own list:

| Preset | Ports |
|---|---|
| Common | 24 ports from the table above (all except 8008 and 8888) |
| Web | 7 ports: 80, 443, 8000, 8008, 8080, 8443, 8888 |
| 1–1024 | Ports 1 to 1024 |

You can also type your own ports, such as `22,80,443` or `1-1024`. One run takes up to 1024 ports, from 1 to 65535. The tool aims at your local network by default and asks for confirmation before it scans a public address.

To find a device to scan, run a scan on the Devices screen first. The app lists each device that answers on your IPv4 /24 network, such as 192.168.1.0/24, with its name and vendor where it can find them. Open one and use its address in the port scan. Results stay on your phone.

## Related checks

- Ping tells you whether the device answers at all and how long it takes. If ICMP is blocked, the app falls back to a TCP check.
- DNS lookup returns A, AAAA and reverse PTR records for a name or address.
- Traceroute shows the hops between your phone and a target.
