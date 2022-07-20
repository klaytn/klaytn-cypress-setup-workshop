---
title: "Telegraf Configuration"
date: 2022-07-14T16:44:50+09:00
weight: 50
pre: "<b>E. </b>"
draft: false
---

{{< line_break >}}
#### 1. To monitor your nodes in Cypress Dashboard, please change the influxdb configuration as below:

##### 1) For both CN and PN,
{{< highlight html >}}
$ grep -A2 "influxdb" /etc/telegraf/telegraf.d/klaytn.conf
[[outputs.influxdb]]
urls = [ "http://13.209.53.161:45560" ]
database = "klaytn_cypress"
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
