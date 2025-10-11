# Session 5a Service Management

[Main Menu](../README.md) | [Session 5a](../session5a/README.md)

## Introduction

This final session will pull together what we have learnt and introduce a few new topics.

This session covers
* HTTPS terminating proxy for OpenNMS using Nginx
* Nginx  monitoring using HttpDataCollector
* Business Service Monitoring
* Brief introduction to Drools
* Brief introduction to Scriptd

from minion 1 172.20.0.1 is the address of the load balancer on the guest operating system
[root@netsnmp_1_1 /]# curl --insecure https://172.20.0.1/wordpress/

curl http://wordpress1/wordpress/?p=1 | grep 'Local Wordpress By Docker'

In this example we will introduce wordpress in a revised network configuration [docker-compose.yaml](../session7/minimal-minion-activemq/docker-compose.yaml)

![alt text](../session5a/images/examplenetwork3.png "Figure examplenetwork3.png")


