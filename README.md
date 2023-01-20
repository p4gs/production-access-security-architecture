# Production access security architecture


| Feature                                                                                                                                     | Most Secure | More Secure | Less Secure | Not Secure |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- | ----------- | ---------- |
| Thing 3                                                                                                                                     |             |             |             |            |
| Ops / SRE has access                                                                                                                        |             |             |             |            |
| Ops / SRE access only through personal break glass accounts                                                                                 |             |             |             |            |
| Ops / SRE access only through JITA                                                                                                          |             |             |             |            |
| Access provided only when an "incident" is open and active (e.g. in ticketing or paging system)                                             |             |             |             |            |
| Access provided only to least-privilege set of production assets (e.g. based on ABAC model, based on assets selected in JITA request, etc.) |             |             |             |            |
| Access granted only after successful FIDO2 MFA at every authN point                                                                         |             |             |             |            |
| Access allowed only from trusted network (e.g. via identity-aware proxy, bastion, VPN, etc.)                                                |             |             |             |            |
| Access allowed only from trusted devices (i.e. company-issued devices authenticated by server)                                              |             |             |             |            |
| Access allowed only from separate privileged access workstation (physical or VDI with LAN/VPC access only)                                  |             |             |             |            |
| Access allowed only from healthy devices (e.g. all security updates installed, endpoint security agent running, etc.)                       |             |             |             |            |
