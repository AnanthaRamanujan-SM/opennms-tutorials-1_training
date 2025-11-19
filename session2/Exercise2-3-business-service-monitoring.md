[Main Menu](../README.md) | [Session 2](../session2/README.md) | [Exercise-2-3-business-service-monitoring](../session2/Exercise-2-3-business-service-monitoring1.md)

# Exercise Business Service Monitoring

It is possible to combine service outages using the Business Service Monitoring feature as shown below.

![alt text](../session2/images/https-loadbalanceServiceTopology.png "Figure https-loadbalanceServiceTopology.png")

For more information see [Business Service Monitoring](https://docs.opennms.com/horizon/33/operation/bsm/introduction.html)
More details of configuring the graph of business services will be covered in a later session. 

Try stopping one wordpress server. 
Wait for 5 minutes and see what alarms occur.

```
docker compose stop wordpress1
```

![alt text](../session2/images/BSM-b-1-alarm.png "Figure BSM-b-1-alarm.png")

Try stopping a second wordpress server. 
Wait for 5 minutes and see what alarms occur.

```
docker compose stop wordpress2
```

![alt text](../session2/images/BSM-b-2-alarms.png "Figure BSM-b-2-alarms.png")

Try stopping all of the wordpress servers. 
Wait for 5 minutes and see what alarms occur.
```
docker compose stop wordpress3
```

![alt text](../session2/images/BSM-b-3-alarms.png "Figure BSM-b-3-alarms.png")

Restart all the wordpress servers and see if the alarms disappear.
```
docker compose up -d
```




