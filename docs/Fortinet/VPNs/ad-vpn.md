# AD-VPN

## General operation

As shown below, once the traffic travels from Spoke 1 to Spoke 2, the three FortiGate devices are involved in the shortcut message interchange.

The hub sends a shortcut offer message to Spoke 1 for a more direct tunnel from Spoke 1 to Spoke 2.

Spoke 1 acknowledges the shortcut offer by sending a shortcut query to the hub.

The hub forwards the shortcut query to Spoke 2, including the WAN IP address of Spoke 2, in this case 100.65.3.113.

Spoke 2 acknowledges the shortcut query and sends a shortcut reply to the hub.

The hub forwards the shortcut reply to Spoke 1.

Spoke 1 and Spoke 2 initiate the tunnel IKE negotiation with the IP address of Spoke 2 sent to ADVPN.

![AD-VPN Diagram](ad-vpn.png)
