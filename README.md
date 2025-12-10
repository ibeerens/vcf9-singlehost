# VCF9 Singlehost configuration

## VCF9 Single host configuration

| VLAN	| Role | IP Address |	Network |
| ---         | ---   | ---         | --- |
| 13	| management | 192.168.13.254/24	| 192.168.13.0 |
| 12	| vmotion	| 10.10.12.1/24	| 10.10.12.0 |
| 50	| vsan | 10.10.50.1/24	| 10.10.50.0 |
| 60	| ESX/NSX Edge TEP (overlay NSX) | 10.10.60.1/24	| 10.10.60.0 |
| 70	| Tier 0 Uplink	| 10.10.70.1/24	| 10.10.70.0 |
| 80	| Kubernets (cluster K8s bare-metal) | 10.10.80.1/24 | 10.10.80.0 |

## Host overview

| Hostname	  | FQDN	| IP Address	| Function |
| ---         | ---   | ---         | --- |
| dc02	| dc02.lab.local |192.168.13.101 | DNS Server and NTP source |
| esx01	| esxi01.lab.local | 192.168.11.11 | Physical ESX Server |
| vcf-depot	| vcf-depot.lab.local	| 192.168.13.62 |	VCF Installer / SDDC Manager |
| vc03 | vcsa03.lab.local | 192.168.13.13	| vCenter Server for Management Domain |
| vcfops01 | vcfops01.lab.local	| 192.168.13.50	| VCF Operations |
| vcfm01 | vcfm01.lab.local | 192.168.13.63 | VCF Operations Fleet Manager |
| vcfopscol01 | vcfopscol01.lab.local	| 192.168.13.64	| VCF Operations Proxy Collector |
| nsx01	| nsx01.lab.local	| 192.168.13.65	| NSX Manager VIP for Management Domain |
| mgmt-nsx01	| mgmt-nsx01.lab.local | 192.168.13.66	| NSX Manager for Management Domain |
| vcfedge01a	| vcfedge01a.lab.local | 192.168.13.67	| NSX Edge 1a for Management Domain |
| vcfedge01b	| vcfedge01b.lab.local | 192.168.13.68	| NSX Edge 1b for Management Domain |
| vcfauto01 | vcfauto01.lab.local	| 192.168.13.69	| VCF Automation |


8.18.5.24967137
