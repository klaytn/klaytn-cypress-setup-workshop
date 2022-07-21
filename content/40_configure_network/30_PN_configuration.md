---
title: "PN static-nodes.json"
date: 2022-07-11T17:55:05+09:00
weight: 30
pre: "<b>C. </b>"
draft: false
---

{{< line_break >}}
#### 2. Modify the static-nodes.json in your PN1 and PN2.

##### Since the information in the static-nodes.json is different for each PN, we will inform each CCO individually by Slack DM.
_** Please refer the diagram below and the docs to understand PNN(Proxy Node Network)._ 
https://docs.klaytn.foundation/klaytn#tiered-networks

> PNN(Proxy Node Network) consists of PNs within the Cypress network topology.   
> Typically, PNs maintain just one connection with a PN in a neighboring Core Cell. The number of peer connections is subject to change depending on the network configuration.

_** Please note that unlike CN, PN uses a static-nodes.json file to find out where to connect._   

![Klaytn_Network_Topology](/images/PNN_topology.png)


{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
