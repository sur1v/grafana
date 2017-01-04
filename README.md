# grafana
just a safe place to store my customs dashboards

------------------------------------------------------------------------
Most of the current plugins to do dashboards with Jenkins are Job centric, leaving behind live monitoring the tool itself. This dashboard provide jobs queue speeds and rates, executors availability, nodes status, host and JVM resource usage.

To gather the metrics from Jenkins you will need some plugins...

Exposes the Jackson 2 API to other Jenkins plugins: https://wiki.jenkins-ci.org/display/JENKINS/Jackson2+API+Plugin Exposes the Codahale Dropwizard Metrics API: https://wiki.jenkins-ci.org/display/JENKINS/Metrics+Plugin Report metrics to Graphite: https://wiki.jenkins-ci.org/display/JENKINS/Metrics+Graphite+Plugin

After plugins reboot Jenkins and go to "Jenkins > Manage Jenkins > Configure System", make sure to define your Graphite hostname, port and for prefix use "jenkins" to make it work almost out of the box ;)
