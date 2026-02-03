# PPPoE Service

## IPv4

```
# Basic Service
Framed-Protocol := PPP
Service-Type := Framed-User

# Static IP
Service-Type := Framed
Framed-IP-Address := 192.0.2.2
Framed-IP-Netmask := 255.255.255.255

# Routed Subnet / "Framed Route"
Framed-Route := "192.0.2.4 255.255.255.248 0.0.0.0"
```

## IPv6

```
# Static IP
Framed-IPv6-Address := 2001:db8:100::1/128

# DNS
DNS-Server-IPv6-Address := <DNS>

# Prefixes from a Pool
Delegated-IPv6-Prefix-Pool := POOL-NAME

# A static prefix
Delegated-IPv6-Prefix := 2001:db8:abcd:1200::/56
```
