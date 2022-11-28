---
title: Broken Authentication and Session Management
author: 
  name: 0xKayala
  link: https://github.com/0xKayala
date:  2022-11-26 00:50
categories: [BROKEN-AUTHENTICATION, SESSION-MANAGEMENT]
tags: [owasp, broken-authentication, session-management,]
math: true
mermaid: true
# Lets start now
---




## Broken Authentication and Session Management


Step by Step Explanation

1st Scenario
📌 Old Session Does Not Expire After Password Change

![01](https://user-images.githubusercontent.com/16838353/204044132-3b5f3235-0fe2-4a55-9844-10aac72567bd.jpeg)
<br>
<br>


2nd Scenario
📌 Session Hijacking (Intended Behaviour)
Impact: If attacker get cookies of victim it will leads to account takeover.

![02](https://user-images.githubusercontent.com/16838353/204044178-ed44c188-a032-40de-a7cf-269a5c3d40e7.jpeg)
<br>
<br>


3rd Scenario
📌 Password reset token does not expire (Insecure Configuration)

![03](https://user-images.githubusercontent.com/16838353/204044237-d08fc801-a9f8-425e-b3fe-3ca024a470cb.jpeg)
<br>
<br>


4th Scenario
📌 Server security misconfiguration 
-> Lack of security headers -> Cache control for a security page

![04](https://user-images.githubusercontent.com/16838353/204044264-9b0a2e64-9a29-4f7d-a16b-955ef38fd00e.jpeg)
<br>
<br>


5th Scenario
📌 Broken Authentication to Email Verification Bypass (P4):
Category: P4 >> Broken Authentication and Session Management >>Failure to Invalidate Session >> On Password Reset and/or Change

![05](https://user-images.githubusercontent.com/16838353/204044316-323548a6-ccae-439b-b060-48d262ebef87.jpeg)
<br>
<br>


6th Scenario
📌 Email Verification Bypass (P3/P4)
Impact: Email Verification Bypass

![06](https://user-images.githubusercontent.com/16838353/204044346-10906664-08b0-44e2-886f-ae4c3ce91ab8.jpeg)
<br>
<br>


7th Scenario
📌 Old Password Reset Token Not Expiring upon Requesting New One (Sometimes P4)
Note: Some Companies won't Accept it as a Valid Issue.

![07](https://user-images.githubusercontent.com/16838353/204044374-42808527-902e-4986-9338-7d45e1230c16.jpeg)
<br>
<br>


8th Scenario
📌 Password Reset Token Not Expiring After Password Change (P4):

![08](https://user-images.githubusercontent.com/16838353/204044395-7c58fef8-a57e-46e9-a3d5-0567c6c46688.jpeg)
<br>
<br>

Thank you guys for Reading this Post - Happy Hunting 🐞

Resources: Google & YouTube

Authors: <a href="https://mobile.twitter.com/FaniMalikHack"> Farhan </a> & Raiders

Credits: <a href="https://mobile.twitter.com/Aacle_"> Abhishek Meena </a>

Follow me: <a href="https://mobile.twitter.com/0xKayala"> Satya Prakash </a>
