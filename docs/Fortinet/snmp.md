# SNMP Configuration

## Fortigates

### HA nodes monitoring

#### Monitor HA Node

In order to monitor a specific node in SNMP in a FGCP cluster :

- Use it's management interface dedicated IP
- Set `ha-direct enable` in the SNMP user config

#### Monitor FGCP cluster

The instruction `ha-direct` must be set at `disable` in order to monitor the whole cluster from a cluster interface.  
Be aware that if you are in a multi-vdom config, you need use an interace belonging to the management vdom.

#### Monitor cluster and each node of a FGCP cluster

In order to monitor both the cluster and each node, you can create one snmp user with `ha-direct` set to `enable` and the other set to `disable`.  
And follow above instructions.

#### References

[SNMP Polling via dedicated HA](https://community.fortinet.com/t5/FortiGate/Technical-Tip-FortiGate-SNMP-polling-via-the-dedicated-HA/ta-p/196034)