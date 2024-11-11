---
title: "Stop the Telegraf service"
date: 2022-07-11T15:16:34+09:00
weight: 20
pre: "<b>B. </b>"
draft: false
---

{{< line_break >}}
##### 2. Stop the Telegraf service, if it is running.
###### 1) For both CN and PN,
{{< highlight html >}}
$ sudo systemctl status telegraf
$ sudo systemctl stop telegraf
$ sudo systemctl status telegraf
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
