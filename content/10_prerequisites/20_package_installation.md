---
title: "Package Installation"
date: 2022-07-11T19:18:57+09:00
weight: 20
pre: "<b>B. </b>"
draft: false
---

{{< line_break >}}

#### 2. Installation of Klaytn packages for CN and PN
_** We've already installed packages during the Pre-cypress stage. If you need to install newly, please refer these documents._
##### 1) Document pages
1. CN - <https://docs.kaia.io/nodes/core-cell/install/install-consensus-nodes/>
2. PN - <https://docs.kaia.io/nodes/core-cell/install/install-proxy-nodes/>
##### 2) Reinstall k*nd caused by version conflict
{{< highlight html >}}
$ sudo su
$ cd /tmp
$ cp /etc/k*nd/conf/k*nd.conf /tmp
$ systemctl stop k*nd
$ aws s3 cp s3://klaytn-packages-repo/packages/rhel/7/kaia/k*nd-v1.0.1-0.el7.x86_64.rpm ./
$ yum remove k*nd -y
$ rpm -Uvh --force k*nd-v1.0.1-0.el7.x86_64.rpm
$ cp k*nd.conf /etc/k*nd/conf/
$ systemctl start k*nd
$ k*n version
{{< /highlight >}}
##### 3) Change yum repo url
{{< highlight html >}}
$ sudo rm /etc/yum.repos.d/klaytn.repo
$ sudo curl -o /etc/yum.repos.d/kaia.repo https://packages.klaytn.net/config/rhel/7/kaia.repo
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.