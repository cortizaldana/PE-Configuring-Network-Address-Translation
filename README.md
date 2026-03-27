# PE-Configuring-Network-Address-Translation

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

# Video 

<!-- Use LinkedIn post to direct to video -->
