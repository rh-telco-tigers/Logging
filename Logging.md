# Show how to check node logs

```bash
#1
oc debug node/master1.nokia.ocp-poc-demo.internal
chroot /host

#2
oc get nodes
oc adm node-logs <node-name>
```

# See what logs are available in masters/workers/infra nodes in /var/log:
```bash
oc adm node-logs --role master --path=/
oc adm node-logs --role worker --path=/
oc adm node-logs --role infra --path=/
```

# Show logs available in a node in /var/log:

# If web console is not up, then where to check :
```bash
oc get co
oc project openshift-console
```

# How to check if master / worker nodes in good state ?
```bash
Web Console
oc get nodes. 
```

# OpenShift Log Forwarder to Kafka
https://srikanthvalluru.medium.com/openshift-log-forwarder-to-kafka-5eb2af6f1528

# OpenShift Log Forwarder to Splunk
https://srikanthvalluru.medium.com/openshift-log-forwarder-to-splunk-3763c5ed3090


