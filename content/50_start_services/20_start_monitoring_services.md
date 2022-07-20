---
title: "Start the monitoring services"
date: 2022-07-11T18:39:03+09:00
weight: 20
pre: "<b>B. </b>"
draft: false
---

{{< line_break >}}
#### 2. Start monitoring services.
##### 1) For both CN and PN, start the Telegraf service.
{{< highlight html >}}
$ sudo systemctl status telegraf
$ sudo systemctl start telegraf
$ sudo systemctl status telegraf
{{< /highlight >}}

##### 2) For both CN and PN, start the Datadog service if it is stopped.
{{< highlight html >}}
$ sudo systemctl status datadog-agent
$ sudo systemctl start datadog-agent
$ sudo systemctl status datadog-agent
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.



