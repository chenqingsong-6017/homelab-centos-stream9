Homelab: CentOS Stream 9 on VirtualBox



Purpose: This homelab is built for RHCSA certification preparation and daily Linux practice.



Environment



Item Specification

Host OS Windows 11

Hypervisor Oracle VirtualBox 7.x

Guest OS CentOS Stream 9 (Minimal Install)

RAM 4 GB

CPU 2 vCPUs

Disk 20 GB (dynamic)



Network Configuration



Interface Type IP Address Purpose

enp0s3 NAT 10.0.2.15 Internet access for package installation

enp0s8 Host-Only 192.168.56.101 SSH access from host machine



Key Services



· SSH: Enabled and running on port 22

· Firewall: firewalld (default zone: public)

· SELinux: Enforcing (default)



SSH Access from Host



```bash

ssh chen@192.168.56.101

```



Verification Commands



```bash

\# Check OS version

cat /etc/redhat-release



\# Check IP addresses

ip -br a



\# Check SSH service status

systemctl status sshd

```



Next Steps



□ RHCSA practice: user/group management

□ RHCSA practice: systemctl service management

□ RHCSA practice: firewall configuration

□ RHCSA practice: LVM and file systems



References



· CentOS Stream 9 Documentation

· RHCSA Exam Objectives



\---



Created by Chen Qingsong on 2026-09-08



