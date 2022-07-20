---
title: "Prepare genesis.json for Cypress network"
date: 2022-07-11T17:10:58+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---

{{< line_break >}}
#### 1. Remove or backup existing genesis.json for Baobab.
##### 1) For CN,
{{< highlight html >}}
$ mv <your_klaytn_home_path>/kcnd/data/genesis.json <your_klaytn_home_path>/kcnd/data/genesis.json.baobab 
{{< /highlight >}}
##### 2) For PN,
{{< highlight html >}}
$ mv <your_klaytn_home_path>/kpnd/data/genesis.json <your_klaytn_home_path>/kpnd/data/genesis.json.baobab
{{< /highlight >}}
{{< line_break >}}

#### 2. Download the genesis.json for Cypress network.
##### 1) For CN,
{{< highlight html >}}
$ curl -X GET https://packages.klaytn.net/cypress/genesis.json -o <your_klaytn_home_path>/kcnd/data/genesis.json
{{< /highlight >}}
##### 2) For PN,
{{< highlight html >}}
$ curl -X GET https://packages.klaytn.net/cypress/genesis.json -o <your_klaytn_home_path>/kpnd/data/genesis.json
{{< /highlight >}}
{{< line_break >}}

#### 3. Check the value of chainId in the genesis.json downloaded.
_** Please note that Cypress network id is 8217._
##### 1) For CN,
{{< highlight html >}}
$ grep "chainId" <your_klaytn_home_path>/kcnd/data/genesis.json
"chainId": 8217,
{{< /highlight >}}
##### 2) For PN,
{{< highlight html >}}
$ grep "chainId" <your_klaytn_home_path>/kpnd/data/genesis.json
"chainId": 8217,
{{< /highlight >}}
{{< line_break >}}

_** If you want to get more information about genesis.json, please refer this link below._   
_https://docs.klaytn.foundation/node/service-chain/references/genesis_

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
