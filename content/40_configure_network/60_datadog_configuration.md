---
title: "Datadog Configuration"
date: 2022-07-20T15:33:50+09:00
weight: 60
pre: "<b>F. </b>"
draft: false
---

{{< line_break >}}
#### 2. For additional monitoring, we are planning to use Datadog as well. Please follow this step for Datadog installation.

##### 1) For CN, 
{{< highlight html >}}
$ cat <<EOF>> dd_vars
DD_API_KEY="DATADOG API KEY"
NETWORK="cypress"
NODE_NAME="<cco_name>-cn-01" 
NODE_TYPE=cn 
INSTANCE=cn 
LOG_DIR="<your_klaytn_home_path>/kcnd/log"
EOF

$ source dd_vars

$ bash -c "$(curl -L https://raw.githubusercontent.com/klaytn/datadog-agent-install./main/install-datadog-agent.sh)"
{{< /highlight >}}
_** DD_API_KEY will be shared with you by Slack DM._   
_** Please use lowercase for NODE_NAME._   
_** For example, ```LOG_DIR = /data/kcnd/log or /data/kcnd/logs, NODE_NAME=cco_name-cn-01```_   

##### 2) For PN,
{{< highlight html >}}
$ cat <<EOF>> dd_vars
DD_API_KEY="DATADOG API KEY"
NETWORK="cypress"
NODE_NAME="<cco_name>-pn-01" or "<cco_name>-pn-02"
NODE_TYPE="pn"
INSTANCE="pn1"
LOG_DIR="<your_klaytn_home_path>/kpnd/log"
EOF

$ source dd_vars

$ bash -c "$(curl -L https://raw.githubusercontent.com/klaytn/datadog-agent-install./main/install-datadog-agent.sh)"
{{< /highlight >}}
_** DD_API_KEY will be shared with you by Slack DM._   
_** Please use lowercase for NODE_NAME._   
_** For example, ```NODE_NAME=cco_name-pn-01 or cco_name-pn-02```_   

#### 3. To allow your nodes to communicate Datadog, please add these IP addresses to the firewall of each node.
##### Port number 443 ```3.233.144.0/20```
##### Port number 10516 ```3.233.152.63/32```

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
