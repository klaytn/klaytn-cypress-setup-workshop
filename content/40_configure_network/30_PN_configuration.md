---
title: "PN static-nodes.json"
date: 2022-07-11T17:55:05+09:00
weight: 30
pre: "<b>C. </b>"
draft: false
---

{{< line_break >}}
#### 2. Check if the static-nodes.json has correct information for your PN.
_** Unlike CN, PN uses a static-nodes.json file to find out where to connect and PNN consists of PNs within the Cypress network topology._
_https://docs.klaytn.foundation/klaytn#tiered-networks_
> Typically, PNs maintain just one connection with a PN in a neighboring Core Cell. The number of peer connections is subject to change depending on the network configuration.
![Klaytn_Network_Topology](/images/klaytn_network_topology.png)


##### 1) For Thrust ,
PN1
{{< highlight html >}}
[
  "CN_KNI_ADDRESS@CN_INTERNAL_IP:PORT?discport=0&ntype=cn"
]
{{< /highlight >}}
PN2
{{< highlight html >}}
[
"CN_KNI_ADDRESS@CN_INTERNAL_IP:PORT?discport=0&ntype=cn"
]
{{< /highlight >}}


{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
