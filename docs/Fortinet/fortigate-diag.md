# Fortigate Debug commands

## BGP

### Get BGP logs

```fortios
diagnose debug reset
diagnose ip router bgp all enable
diagnose ip router bgp level info
diagnose debug enable
diag ip router bgp set-filter neighbor a.b.c.d
```

### Useful links

- [Technical Tip: Capture BGP debugs for a specific neighbor (Fortinet Community)](https://community.fortinet.com/t5/FortiGate/Technical-Tip-Capture-BGP-debugs-for-a-specific-neighbor/ta-p/352981)
- [FortiGate BGP Troubleshooting Guide (boll.ch blog)](https://blog.boll.ch/fortigate-bgp-troubleshooting-guide/)
- [Technical Tip: Verify BGP Prefix received from peer with BGP debug (Fortinet Community)](https://community.fortinet.com/t5/FortiGate/Technical-Tip-Verify-BGP-Prefix-received-from-peer-with-BGP/ta-p/230377)

## Link with FMG

**On FortiManager**

```fortios
diag debug service sys 255
diag debug application depmanager 255
diag debug enable
diag fwmanager fwm-log
diag debug application fgfmsd 255
```

**On FortiGate**

```fortios
diagnose debug cli 8
diag debug application fgfmd 255
diag debug enable
```

## Packets

### Sniffer

`diagnose sniffer packet any "" 4 ? a/l`

### Flow

```fortios
diagnose debug flow filter <filter> <-- Can be used multiple times
diagnos debug enable
diagnose debug flow trace start xxx
diagnose debug flow trace stop
```

## SNMP

### Debug commands

```FortiOS
diagnose debug disable
diagnose debug reset
diagnose test application snmpd -1
diagnose debug enable 
```
