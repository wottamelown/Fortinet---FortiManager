# Fortinet---FortiManager

1. port 1 is default mgmt int
2. 192.168.1.99 is the management IP.
3. config system int > show > edit port > set allow access http https >

-- GUI Overview --

1. Device Manager: Add Devices, VPN Monitor, SD-WAN Monitor, Provisioning Templates.
2. Policy & Objects: Creating firewall policies & objects
3. AP Manager: Used for multiple APs management.
4. VPN Manager: used for IPSec, SSL VPNs. etc etc
5. Fabric View: Topology physical and logical
6. FortiGuard: To see license and upgrade the firewalls.
7. Fortiswitch Manager: to change the ports of fsw.
8. Reports: Generate reports.

-- Important Topics --

9. We can create ADOMs to create logical grouping according to the requirements.
10. Device Registration: Discover Device using IP, ADD S/N then IP, using CSV.
11. We can do registration using FGT as well using Fabric Connectors. 
12. 

-- Provisioning Templates --

13. We can create System templates, SD-WAN Templates, IPSec Tunnel Templates, BGP, Static Route Templates, CLI Templates
14. Then we have Template Groups to combine all the above templates and push it to the devices.
15. We can import the templates from already available devices FGTs and then make a templates.
16. We can assign the templates then go to device manager to install the templates.

-- Device Groups --

17. Device Groups > Managed ForitGates > Create New Group.

-- Scripts --

18. There are 2 types of scripts CLI and TCL.
19. We can create a script to configure using CLI ZTP and then push it to devices to update the configuration.

-- Revision History --
20. Revision history means to check the history and revert back if something goes wrong. 
21. We can check the revision history by going to the FGT in device manager and then click on it then Device Revisions. 
22. The updates shows (Auto-Update, Out Of Sync, Modified, Modified (recent auto updated)

-- Policy & Objects --

23. These are like the firewall policies which we can set per device or per group.
24. Policy Package is a firewall rule. Objects are the IP addresses, FQDNs, Security Profiles, Virtual Servers etc etc.
25. Normalized Interfaces are different int configurations for each device.
26. First Step is to create normalized Interface For LAN, WAN
27. Then we can create Policy Package and then create firewall policy.  
28. Last step if to add the installation targets and then install policy package.

-- VPN Manager --
29. Forti Manager supports Full Mesh, Star, Dial Up. 
30. Mesh means all devices has a tunnel to other HQ - DC, DC - Site, HQ - Site.
31. Star means Sites will forward the traffic to HUB and send all the traffic to HQ. 
32. 
