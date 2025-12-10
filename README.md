# vcf9-singlehost
VCF9 Single host

+ --- + --- + ---- +
VLAN	Role	IP Address	Network
30	management	192.168.79.254/24	192.168.79.0
40	vmotion	10.10.40.1/24	10.10.40.0
50	vsan	10.10.50.1/24	10.10.50.0
60	ESX/NSX Edge TEP (overlay NSX)	10.10.60.1/24	10.10.60.0
70	Tier 0 Uplink	10.10.70.1/24	10.10.70.0
80	Kubernets (cluster K8s bare-metal)	10.10.80.1/24	10.10.80.0


| Hostname	  | FQDN	| IP Address	| Function |
| ---         | ---   | ---         | --- |
| dc02	| dc02.lab.local |192.168.13.101 | DNS Server and NTP source |
| esx01	| esxi01.lab.local | 192.168.11.11 | Physical ESX Server |
| vcf-depot	| vcf-depot.lab.local	| 192.168.13.62 |	VCF Installer / SDDC Manager |
| vc03 | vcsa03.lab.local 192.168.13.13	| vCenter Server for Management Domain |
| vcfops01 | vcfops01.lab.local	| 192.168.13.50	| VCF Operations |
| vcfm01 | vcfm01.lab.local | 192.168.13.63 | VCF Operations Fleet Manager |
| vcfopscol01 | vcfopscol01.lab.local	| 192.168.13.64	| VCF Operations Proxy Collector |
| nsx01	| nsx01.lab.local	| 192.168.13.65	| NSX Manager VIP for Management Domain |
| mgmt-nsx01	| mgmt-nsx01.lab.local	| 192.168.13.66	| NSX Manager for Management Domain |
| edge01a	| edge01a.virtualizandoaju.com.br	| 192.168.79.17	| NSX Edge 1a for Management Domain |
| edge01b	| edge01b.virtualizandoaju.com.br	| 192.168.79.18	| NSX Edge 1b for Management Domain |
| auto01 | auto01.virtualizandoaju.com.br	| 192.168.79.30	| VCF Automation |


8.18.5.24967137
