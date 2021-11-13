# Scenario 2 - Solution

## Objective

Given the specs of a server as below: 
* 4 times Intel(R) Xeon(R) CPU E7-4830 v4 @ 2.00GHz
* 64GB of ram
* 2 TB HDD disk space
* 2 x 10Gbit/s nics

The server is used for SSL offloading and proxies around 25000 requests per second. 

Determine the following:

1. Which metrics are interesting to monitor?
2. How would you monitor those metrics?
3. What are the challenges of monitoring those metrics?

## Answers

1. Which metrics are interesting to monitor in the given situation? 
   1. **CPU load** - as SSL offloading is CPU sensitive process. 
   2. **File descriptor** - it decides the number TCP connections
   3. **Open connections** - too many TCP open connections can cause server degradation
   4. **Memory (RAM)** - too many transactions can also result to server degradation 
   5. **Network in/network out latency** - as a single server would cause high network load resulting to a bottle neck situation. 
   6. **Network in/network out bytes** - as the larger packet size would congest the network

2. How would you monitor those metrics?
    
    These metrics can be monitored by custom cron jobs running on the server itself or a better way would be to use 3rd party tools that install agents to report the same eg: Datadog, Nagios or Metricbeat to name a few.

3. What are the challenges of monitoring this?
    
    The metrics mentioned above can be monitored by either using custom scripts executed by cron jobs or by 3rd party tools like Datadog, Nagios or Metricbeat to name a few but the main challenge is to collect these metrics in real-time or in other words by the second. 
    Though there are unconventional ways to collect the above mentioned metrics by the second using a cron job a better solution would to be to use one of the reliable 3rd party tool/service/application to do the same.