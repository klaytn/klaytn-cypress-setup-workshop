---
title: "Node Initialization"
date: 2022-07-11T17:23:03+09:00
weight: 40
pre: "<b>D. </b>"
draft: false
---

{{< line_break >}}
#### 1. Now, we will initialize each node using the Cypress genesis file.

##### 1) For CN,
{{< highlight html >}}
$ cd <your_klaytn_home_path>/kcnd/data
$ kcn --networkid 8217 init --datadir <your_klaytn_home_path>/kcnd/data genesis.json
{{< /highlight >}}

##### 2) For PN,
{{< highlight html >}}
$ cd <your_klaytn_home_path>/kpnd/data
$ kpn --networkid 8217 init --datadir <your_klaytn_home_path>/kpnd/data genesis.json
{{< /highlight >}}
{{< line_break >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
