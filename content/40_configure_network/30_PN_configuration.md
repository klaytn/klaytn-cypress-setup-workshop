---
title: "PN static-nodes.json"
date: 2022-07-11T17:55:05+09:00
weight: 30
pre: "<b>C. </b>"
draft: false
---

{{< line_break >}}
#### 2. Modify the static-nodes.json in your PN1 and PN2.

> PNN(Proxy Node Network) consists of PNs within the Cypress network topology.
> > Typically, PNs maintain just one connection with a PN in a neighboring Core Cell. The number of peer connections is subject to change depending on the network configuration.

##### Since the information in static-nodes.json is different for each PN, we will inform each CCO individually.    
_** Please refer below diagram and the docs. - https://docs.klaytn.foundation/klaytn#tiered-networks_   
_** Unlike CN, PN uses a static-nodes.json file to find out where to connect._   

![Klaytn_Network_Topology](/images/klaytn_network_topology.png)


{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
