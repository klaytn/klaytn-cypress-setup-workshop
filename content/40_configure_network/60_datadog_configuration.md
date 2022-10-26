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
$ DD_API_KEY="DATADOG API KEY" HOST_NAME="CN HOSTNAME" NODE_TYPE=cn INSTANCE=cn LOG_DIR="<your_klaytn_home_path>/kcnd/log/kcnd.out" bash -c "$(curl -L https://raw.githubusercontent.com/klaytn/datadog-agent-install./main/install-datadog-agent.sh)"
{{< /highlight >}}
_** DD_API_KEY will be shared with you by Slack DM._   
_** Please use lowercase, then append 'cn-01' for HOST_NAME_   
_** For example, ```LOG_DIR = /data/kcnd/log/kcnd.out or /data/kcnd/logs/kcnd.out, HOST_NAME=cco_name-cn-01```_   

##### 2) For PN,
{{< highlight html >}}
$ DD_API_KEY="DATADOG API KEY" HOST_NAME="PN HOSTNAME" NODE_TYPE=pn INSTANCE=pn1 bash -c "$(curl -L https://raw.githubusercontent.com/klaytn/datadog-agent-install./main/install-datadog-agent.sh)"
{{< /highlight >}}
_** DD_API_KEY will be shared with you by Slack DM._   
_** Please use lowercase, then append 'pn-01' or 'pn-02' for HOST_NAME_   
_** For example, ```HOST_NAME=cco_name-pn-01 or cco_name-pn-02```_   

#### 3. To allow your nodes to communicate Datadog, please add these IP addresses to the firewall of each node.
##### Port number 443 ```3.233.144.0/20```
##### Port number 10516 ```3.233.152.63/32```

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
