# OSS-Monitor-and-Alert-System
Monitor  &amp; Alert with Opensearch is an monintoring tool which will provide a Monitoring Dasboard and provide alerts based on some of the common metrics.
It will support the following modules to monitor
1. Linux
2. Unix
3. Windows
    * Note: It can support all the [modules](https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-modules.html) currently supported by metricbeat in the future.

![FLow Diagram](fdiagram.png)


Installation Process
---

The installation consist of two steps
1. Download the server_config_template.cfg and modify the config details.
2. Installing the open search cluster with the following commands
   ```
   make install-server -config=<path_to_server_config>
   ```
3. Download client_config_template.cfg
4. Installing the metricbeat-oss(+logstash - maybe) clients to the Linux/Unix/Windows system
   ```
   make install-client -config=<path_to_client_config>
   ```


