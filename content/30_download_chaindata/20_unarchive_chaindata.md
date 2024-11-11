---
title: "Extract the chaindata"
date: 2022-07-11T15:43:06+09:00
weight: 20
pre: "<b>B. </b>"
draft: false
---

{{< line_break >}}
##### 2. Extract the chaindata downloaded to the DATA_DIR.

###### 1) For CN,
{{< highlight html >}}
$ tar -C <your_kaia_home_path>/kcnd/data -xvf kaia-mainnet-pruning-chaindata-20241109011112.tar.gz --exclude klay/chaindata/receipts
{{< /highlight >}}

###### 2) For PN,
{{< highlight html >}}
$ tar -C <your_kaia_home_path>/kpnd/data -xvf kaia-mainnet-pruning-chaindata-20241109011112.tar.gz --exclude klay/chaindata/receipts
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
