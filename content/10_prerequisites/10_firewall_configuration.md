---
title: "Firewall Configuration"
date: 2022-07-11T19:18:45+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---
{{< line_break >}}

#### 1. *(Only for CN)* Firewall configuration

##### 1) If Baobab validation is completed, remove below Klaytn CN's IP addresses of Baobab from your firewall configuration.
```54.180.180.202```   
```54.180.18.176```   
```52.79.134.72```   
```52.78.232.39```
{{< line_break >}}

##### 2) For communication and multichannel across CCO CNs in the Cypress network, TCP ```32323-32324``` and UDP ``` 32323 ``` from existing CCO's CNs should be allowed in your CN firewall configuration.
_** The existing CCO's CNs IP addresses will be provided by Slack DM._

{{< line_break >}}
##### 3) For communication and multichannel across Bootnode in the Cypress network, UDP ``` 32323 ``` from existing CCO's CNs should be allowed in your CN firewall configuration.
_** The existing Bootnode IP addresses will be provided by Slack DM._

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
