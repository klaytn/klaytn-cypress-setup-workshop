---
title: "Download the latest Cypress chaindata"
date: 2022-07-11T15:42:53+09:00
weight: 10
pre: "<b>A. </b>"
draft: false
---

{{< line_break >}}
#### 1. Download the latest chaindata snapshot from the Cypress snapshot archive.
##### 0) Before proceeding, please check if your disk space is enough to store and extract the Cypress chaindata.
_** You can refer to the chaindata size via **[Cypress snapshot archive](https://packages.klaytn.net/cypress/chaindata/)** where the Cypress chaindata snapshots have been snapshotted._   
{{< line_break >}}

##### 1) For CN
_** Please note that this step will take a lot of time to download since snapshot is more than 1.4 TB. If you want to reduce the time, please refer the next step._   
_** The latest chaindata name can be different with this example due to the date information._
{{< highlight html >}}
$ URL=`curl -s https://packages.klaytn.net/cypress/pruning-chaindata/  |grep latest |awk -F'"' '{print $2}'`
$ echo $URL
https://s3.ap-northeast-2.amazonaws.com/klaytn-chaindata/cypress/pruning/klaytn-cypress-pruning-chaindata-20240131010111.tar.gz
$ wget $URL
{{< /highlight >}}
##### 2) For PN2
{{< highlight html >}}
$ URL=`curl -s https://packages.klaytn.net/cypress/pruning-chaindata/ |grep latest |awk -F'"' '{print $2}'`
$ echo $URL
https://s3.ap-northeast-2.amazonaws.com/klaytn-chaindata/cypress/pruning/klaytn-cypress-pruning-chaindata-20240131010111.tar.gz
$ wget $URL
{{< /highlight >}}

##### 2) Optional - If you want to save the time for downloading, you can consider using ```axel``` command.   
_**[Axel](https://github.com/axel-download-accelerator/axel) tries to accelerate the download process by using multiple connections per file._
##### 1) For CN and PN1
{{< highlight html >}}
(Amazon Linux 2) $ sudo amazon-linux-extras install epel
(CentOS) $ sudo yum install epel-release -y
$ sudo yum install axel -y
$ URL=`curl -s https://packages.klaytn.net/cypress/pruning-chaindata/ |grep latest |awk -F'"' '{print $2}'`
$ echo $URL
https://s3.ap-northeast-2.amazonaws.com/klaytn-chaindata/cypress/pruning/klaytn-cypress-pruning-chaindata-20240131010111.tar.gz
$ axel -n8 $URL
{{< /highlight >}}
##### 2) For PN2
{{< highlight html >}}
(Amazon Linux 2) $ sudo amazon-linux-extras install epel
(CentOS) $ sudo yum install epel-release -y
$ sudo yum install axel -y
$ URL=`curl -s https://packages.klaytn.net/cypress/pruning-chaindata/ |grep latest |awk -F'"' '{print $2}'`
$ echo $URL
https://s3.ap-northeast-2.amazonaws.com/klaytn-chaindata/cypress/pruning/klaytn-cypress-pruning-chaindata-20240131010111.tar.gz
$ axel -n8 $URL
{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
