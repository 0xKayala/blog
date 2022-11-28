---
title: SNMP Enumeration
author: 
  name: 0xKayala
  link: https://github.com/0xKayala
date:  2022-11-26 23:55
categories: [SNMP-Enumeration,]
tags: [snmp-enumeration,]
math: true
mermaid: true
# Lets start now
---



## SNMP Enumeration

![SNMP Enumeration](https://user-images.githubusercontent.com/16838353/204099544-ef3538c9-cb64-43cc-a37f-86abcc96122c.jpeg)

#SNMP-Check
<br>
snmp-check ip
<br>
snmp-check $IP
<br>
snmpcheck -t $IP -c public
<br>
snmpcheck -t ip.X -c public
<br>

![image](https://user-images.githubusercontent.com/16838353/204102846-e468f255-f64f-496f-a752-949818af1152.png)
<br>
![image](https://user-images.githubusercontent.com/16838353/204102972-928d5f7c-1eaa-45f6-bf6a-38fd9ed87c6e.png)
<br>

#onesixtyone
<br>
onesixtyone -c names -i hosts
<br>

![image](https://user-images.githubusercontent.com/16838353/204103003-bb6699b2-b8b4-416d-b2dc-b3796352b3b9.png)
<br>

#SNMPWALK
<br>
snmpwalk -c public -v1 $IP
<br>

![image](https://user-images.githubusercontent.com/16838353/204103216-6c63ac1a-42e7-498d-8ffd-1a780a20a871.png)
<br>
![image](https://user-images.githubusercontent.com/16838353/204103228-0eb8e6b0-6f00-490f-8df5-9c85b78f862f.png)
<br>
![image](https://user-images.githubusercontent.com/16838353/204103233-bc3df4f8-b87c-4f47-b3d1-c8f724757c4f.png)
<br>
![image](https://user-images.githubusercontent.com/16838353/204103241-a3b75d7f-f103-4c1d-a956-81709c229248.png)
<br>

#SNMPENUM
<br>
perl snmpenum.pl $IP public windows. txt
<br>

![image](https://user-images.githubusercontent.com/16838353/204103248-2dfd9bf4-a83b-461d-bf3f-63538450a77f.png)
<br>

#NMAP_SCRIPTS
<br>
nmap -р 88 --script krb5-enum-users --script-args krb5-enum-users.realm='domain.local' ,userdb=/usr/share/wordlists/SecLists/Usernames/top_shortlist.txt x.x.x.x
<br>

![image](https://user-images.githubusercontent.com/16838353/204103796-e200d8c8-d66e-4710-9766-0ca58a52d50d.png)
<br>

nmap -vv -sV -sU -Pn -р 161,162 --script=snmp-netstat,snmp-processes $IP
<br>

![image](https://user-images.githubusercontent.com/16838353/204104089-6402a151-e96e-4847-a7b4-0b4d4a15a4d0.png)
<br>

nmap -sU -p 161 --script /usr/share/nmap/scripts/snmp-win32-users.nse $IP
<br>

![image](https://user-images.githubusercontent.com/16838353/204104165-0204e933-8d12-4c82-b208-24bdda15eb8d.png)

<br>

Thank you guys for Reading this Post - Happy Hunting 🐞

Credits: <a href="https://mobile.twitter.com/Aacle_"> Abhishek Meena </a>

Follow me: <a href="https://mobile.twitter.com/0xKayala"> Satya Prakash </a>
