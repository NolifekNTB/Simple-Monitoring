Set up a basic monitoring dashboard using Netdata.

task: https://roadmap.sh/projects/simple-monitoring-dashboard

<br><br>

1. Install netdata using this command:
   
 ``` wget -O /tmp/netdata-kickstart.sh https://get.netdata.cloud/kickstart.sh && sh /tmp/netdata-kickstart.sh```

 2. Run in browser using this IP address:

``` http://localhost:19999 ```

3. Add new custom alert

a) Create new configuration file in "/etc/netdata/health.d" - ``` sudo ../edit-config cpu_usage.conf ```

b) Update active alerts - ``` netdatacli reload-health ```
