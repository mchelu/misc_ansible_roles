# misc_ansible_roles
A collection of usefull ansible roles for configuring Cisco equipment

**configure_specific_interfaces** -> selects all the interfaces on the switch that match the criteria described in the regex (type,status,VLAN) and applies config only to those interfaces. 

**vlan config** -> simplest and fastest way of configuring VLANS in bulk on a Cisco device

**interface_config_clone**-> provide a config file from an older device and the playbook parses the interfaces and applies the same config on a new switch. It can handle various cases where the interface names don't match and it configures the uplinks separately. Good when migrating to a different model. To deploy use deploy.yml as it will prompt for some information before the playbook runs.
