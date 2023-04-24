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

##### 2) Only for CN,
1. Change the interval time of Telegraf agent from 10s to 1s.   
{{< highlight html >}}
$ cat /etc/telegraf/telegraf.conf | grep -v '^\s*$\|^\s*\#' | grep interval
interval = "1s"
round_interval = true
flush_interval = "1s"
{{< /highlight >}}

2. Create a new configuration file klaytn_log.conf for monitoring Klaytn log, and copy/paste the below content.
{{< highlight html >}} 
$ vi /etc/telegraf/telegraf.d/klaytn_log.conf
[[inputs.tail]]
# please use your DIR of the log
files = ["<your_klaytn_home_path>/log/kcnd.out"]

## Read files that currently exist from the beginning. Files that are created
## while telegraf is running (and that match the "files" globs) will always
## be read from the beginning.
from_beginning = false

## Method used to watch for file updates. Can be either "inotify" or "poll".
watch_method = "inotify"

name_override = "klaytn_log"
data_format = "value"
data_type = "string"

[[outputs.influxdb]]
urls = [ "http://13.209.53.161:45560" ]
database = "klaytn_logs"

{{< /highlight >}}

{{< line_break >}}
If you finish this step, please click the next button ```>``` on the right side of this page.
