# Configuring-Network-Address-Translation

# Bridge Communication To The Outside

- KVM machine has once NIC interface
- I need to allow the traffic from all bridges to go out through that only interface
- NAT will allow me to route the traffic out from the KVM Host through firewalld policies

- <a href="https://youtu.be/BO9x8ZJe3mg"> YouTube: Configuring Network Address Translation </a>

# Commands Issued To Configure NAT

```
firewall-cmd --new-policy=isl-to-public --permanent
```

```bash
firewall-cmd --policy=isl-to-public --add-ingress-zone=isl --permanent
```

```bash
firewall-cmd --policy=isl-to-public --add-egress-zone=public --permanent
```

```bash
firewall-cmd --policy=isl-to-public --add-masquerade --permanent
```

```bash
firewall-cmd --reload
```

