---
title: "Stop the Kaia service"
date: 2022-07-11T15:16:17+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---

{{< line_break >}}
##### 1. Stop the Kaia service, if it is running.
###### 1) For CN,
{{< highlight html >}}
$ sudo systemctl status kcnd
$ sudo systemctl stop kcnd
$ sudo systemctl status kcnd
{{< /highlight >}}

###### 2) For PN,
{{< highlight html >}}
$ sudo systemctl status kpnd
$ sudo systemctl stop kpnd
$ sudo systemctl status kpnd
{{< /highlight >}}

###### 3) If the services are not installed from ```yum```, you can stop the service like below,
{{< highlight html >}}
$ sudo <installation_path>/kcnd status
$ sudo <installation_path>/kcnd stop
$ sudo <installation_path>/kcnd status
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
