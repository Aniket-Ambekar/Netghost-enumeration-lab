# NETGHOST-01 Writeup

## Challenge 1 – Ghost Hunt

Command referenced:
nmap -sn 192.168.10.0/24

Flag:
NETGHOST{ping_sweep_reveals_all}

---

## Challenge 2 – Open Doors

curl -I http://192.168.10.10

Flag:
NETGHOST{banner_grab_ftw}

---

## Challenge 3 – FTP Fingerprint

nc 192.168.10.20 21

Flag:
NETGHOST{vsftpd_anon_exposes_banner}

---

## Challenge 4 – OS Oracle

nmap -O 192.168.10.30

Flag:
NETGHOST{linux_4.15_os_detected}

---

## Challenge 5 – Service Census

nmap -sV -sC --script=smb-os-discovery 192.168.10.0/24

Flag:
NETGHOST{smb_enum_complete}
