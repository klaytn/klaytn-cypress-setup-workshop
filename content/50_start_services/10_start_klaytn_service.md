---
title: "Start the Kaia services"
date: 2022-07-11T18:37:31+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---

{{< line_break >}}
##### 1. Start the Kaia service, if it is running.
###### 1) For CN,
{{< highlight html >}}
$ sudo systemctl status kcnd
$ sudo systemctl start kcnd
$ sudo systemctl status kcnd
{{< /highlight >}}

###### 2) For PN,
{{< highlight html >}}
$ sudo systemctl status kpnd
$ sudo systemctl start kpnd
$ sudo systemctl status kpnd
{{< /highlight >}}

###### 3) If the services are not installed from ```yum```, you can start the service like below,
{{< highlight html >}}
$ sudo <installation_path>/kcnd status
$ sudo <installation_path>/kcnd start
$ sudo <installation_path>/kcnd status
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
