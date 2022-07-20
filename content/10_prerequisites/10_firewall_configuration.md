---
title: "Firewall Configuration"
date: 2022-07-11T19:18:45+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---
{{< line_break >}}

#### 1. *(Only for CN)* Firewall configuration

##### 1) If Baobab validation is completed, remove below Klaytn CN's IP address of Baobab from your firewall ingress rule.
```54.180.180.202```   
```54.180.18.176```   
```52.79.134.72```   
```52.78.232.39```

##### 2) For communication and multichannel between Cypress CN, allow TCP ```32323-32324``` with below IP addresses to your firewall ingress rule.
```52.187.181.245```
```13.250.156.19```
```18.181.103.22```
```13.251.72.113```
```15.164.153.242```
```52.78.129.138```
```183.110.37.118```
```3.114.52.253```
```13.115.105.184```
```3.112.138.154```
```13.124.195.223```
```52.68.240.46```
```54.254.44.48```
```3.37.228.174```
```3.1.128.148```
```52.221.66.32```
```13.250.248.137```
```52.194.171.123```
```18.136.27.69```
```121.53.201.23```
```223.130.161.81```
```121.53.201.21```
```46.137.252.23```
```13.209.36.151```
```110.76.140.22```
```49.50.160.250```
```15.164.2.23```
```18.182.254.228```
```52.78.134.8```
```18.141.124.207```
```15.164.144.217```
```13.213.141.240```
```20.222.4.64```
```54.255.230.170```
```52.197.133.145```
```54.255.162.46```
```3.34.162.243```

##### 3) Additionally, it is required to allow UDP ``` 32323 ``` with the same IP addresses to your firewall ingress rule.
_** The same IP addresses in the previous step should be added._

{{< line_break >}}   
*Please note that the above IP addresses are attached to other CCO CNs.*

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
