To import the template which is stored as XML just go to the Zabbix -> Configuration -> Templates -> Import and chose the xml file.

**zbx_vmware_templates.xml** - Template which is working with Zabbix 4.0 LTS to monitor VMware vCenter Server 6.7.0, this version of template has additional Items and Triggers configured thanks to the great tutorial posted on https://bestmonitoringtools.com/vmware-monitoring-with-zabbix-esxi-vcenter-vm-vsphere/

Item protoypes:
  - Free space on datastore (bytes) for Hypervisor
  - CPU Usage (%) for Guest and Hypervisor
  - Memory usage (%) for Guest and Hypervisor
  - CPU Ready Readiness % for Hypervisor
  - CPU Ready Summation for Hypervisor
  - Time until datastore is 100% full for Hypervisor

Trigger prototypes:
  - Free space is less than 5% on datastore for Hypervisor
  - Free space is less than % value (below 5) on datastore, there is space left of total space and for timeframe datastore will be 100% full! for Hypervisor
  - Free space is less than 5% on filesystem for Guest

Graph protoypes:
  - Average read/write latency of the datastore for Hypervisor
  - Free space on datastore (bytes) for Hypervisor
