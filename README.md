# grafana
just a safe place to store my customs dashboards

------------------------------------------------------------------------
***	jenkins-performance-and-health-overview_rev1.json
Most of the current plugins to do dashboards with Jenkins are Job centric, leaving behind live monitoring the tool itself. This dashboard provide jobs queue speeds and rates, executors availability, nodes status, host and JVM resource usage.

To gather the metrics from Jenkins you will need some plugins...

Exposes the Jackson 2 API to other Jenkins plugins: https://wiki.jenkins-ci.org/display/JENKINS/Jackson2+API+Plugin Exposes the Codahale Dropwizard Metrics API: https://wiki.jenkins-ci.org/display/JENKINS/Metrics+Plugin Report metrics to Graphite: https://wiki.jenkins-ci.org/display/JENKINS/Metrics+Graphite+Plugin

After plugins reboot Jenkins and go to "Jenkins > Manage Jenkins > Configure System", make sure to define your Graphite hostname, port and for prefix use "jenkins" to make it work almost out of the box ;)

------------------------------------------------------------------------
*** VMware_vCenter_Performance_and_Health.json
This is a custom performance and health dashboard that will work with SexiGraf https://github.com/sexibytes/sexigraf appliance for active monitoring of vCenter, with multiple clusters support. The goal was provide real KPIs at glance, like CPU and RAM contention not abailable in the default dashboards. Now is calculated on the fly (based on refresh interval), in the same way that you can get the metric from vRealize Operations, but free ;)
