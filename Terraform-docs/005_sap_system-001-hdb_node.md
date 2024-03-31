<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | >= 3.54 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_azurerm.dnsmanagement"></a> [azurerm.dnsmanagement](#provider\_azurerm.dnsmanagement) | >= 3.54 |
| <a name="provider_azurerm.main"></a> [azurerm.main](#provider\_azurerm.main) | >= 3.54 |

## Modules

hdb_node

## Resources

| Name | Type |
|------|------|
| [azurerm_availability_set.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/availability_set) | resource |
| [azurerm_lb.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb) | resource |
| [azurerm_lb_backend_address_pool.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_backend_address_pool) | resource |
| [azurerm_lb_probe.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_probe) | resource |
| [azurerm_lb_rule.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/lb_rule) | resource |
| [azurerm_linux_virtual_machine.vm_dbnode](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/linux_virtual_machine) | resource |
| [azurerm_managed_disk.cluster](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/managed_disk) | resource |
| [azurerm_managed_disk.data_disk](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/managed_disk) | resource |
| [azurerm_managed_disk.kdump](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/managed_disk) | resource |
| [azurerm_netapp_volume.hanadata](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/netapp_volume) | resource |
| [azurerm_netapp_volume.hanalog](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/netapp_volume) | resource |
| [azurerm_netapp_volume.hanashared](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/netapp_volume) | resource |
| [azurerm_netapp_volume_group_sap_hana.avg_HANA](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/netapp_volume_group_sap_hana) | resource |
| [azurerm_network_interface.nics_dbnodes_admin](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/network_interface) | resource |
| [azurerm_network_interface.nics_dbnodes_db](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/network_interface) | resource |
| [azurerm_network_interface.nics_dbnodes_storage](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/network_interface) | resource |
| [azurerm_network_interface_application_security_group_association.db](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/network_interface_application_security_group_association) | resource |
| [azurerm_network_interface_backend_address_pool_association.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/network_interface_backend_address_pool_association) | resource |
| [azurerm_private_dns_a_record.db](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_a_record) | resource |
| [azurerm_role_assignment.role_assignment_msi](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_role_assignment.role_assignment_msi_ha](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_virtual_machine_data_disk_attachment.cluster](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_data_disk_attachment) | resource |
| [azurerm_virtual_machine_data_disk_attachment.kdump](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_data_disk_attachment) | resource |
| [azurerm_virtual_machine_data_disk_attachment.vm_dbnode_data_disk](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_data_disk_attachment) | resource |
| [azurerm_virtual_machine_extension.hdb_linux_extension](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_extension) | resource |
| [azurerm_virtual_machine_extension.monitoring_defender_db_lnx](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_extension) | resource |
| [azurerm_virtual_machine_extension.monitoring_extension_db_lnx](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/virtual_machine_extension) | resource |
| [azurerm_availability_set.hdb](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/availability_set) | data source |
| [azurerm_netapp_account.workload_netapp_account](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/netapp_account) | data source |
| [azurerm_netapp_pool.workload_netapp_pool](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/netapp_pool) | data source |
| [azurerm_netapp_volume.hanadata](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/netapp_volume) | data source |
| [azurerm_netapp_volume.hanalog](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/netapp_volume) | data source |
| [azurerm_netapp_volume.hanashared](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/netapp_volume) | data source |
| [azurerm_subnet.ANF](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/subnet) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_NFS_provider"></a> [NFS\_provider](#input\_NFS\_provider) | Describes the NFS solution used | `string` | n/a | yes |
| <a name="input_admin_subnet"></a> [admin\_subnet](#input\_admin\_subnet) | Information about SAP admin subnet | `any` | n/a | yes |
| <a name="input_anchor_vm"></a> [anchor\_vm](#input\_anchor\_vm) | Deployed anchor VM | `any` | `null` | no |
| <a name="input_cloudinit_growpart_config"></a> [cloudinit\_growpart\_config](#input\_cloudinit\_growpart\_config) | A cloud-init config that configures automatic growpart expansion of root partition | `any` | n/a | yes |
| <a name="input_custom_disk_sizes_filename"></a> [custom\_disk\_sizes\_filename](#input\_custom\_disk\_sizes\_filename) | Disk size json file | `string` | `""` | no |
| <a name="input_database"></a> [database](#input\_database) | n/a | `any` | n/a | yes |
| <a name="input_database_dual_nics"></a> [database\_dual\_nics](#input\_database\_dual\_nics) | Defines if the HANA DB uses dual network interfaces | `bool` | `true` | no |
| <a name="input_database_server_count"></a> [database\_server\_count](#input\_database\_server\_count) | The number of database servers | `number` | `1` | no |
| <a name="input_database_use_premium_v2_storage"></a> [database\_use\_premium\_v2\_storage](#input\_database\_use\_premium\_v2\_storage) | If true, the database tier will use premium storage | `bool` | n/a | yes |
| <a name="input_database_vm_admin_nic_ips"></a> [database\_vm\_admin\_nic\_ips](#input\_database\_vm\_admin\_nic\_ips) | If provided, the database tier will be configured with the specified IPs (admin subnet) | `any` | n/a | yes |
| <a name="input_database_vm_db_nic_ips"></a> [database\_vm\_db\_nic\_ips](#input\_database\_vm\_db\_nic\_ips) | If provided, the database tier will be configured with the specified IPs | `any` | n/a | yes |
| <a name="input_database_vm_db_nic_secondary_ips"></a> [database\_vm\_db\_nic\_secondary\_ips](#input\_database\_vm\_db\_nic\_secondary\_ips) | If provided, the database tier will be configured with the specified IPs as secondary IPs | `any` | n/a | yes |
| <a name="input_database_vm_storage_nic_ips"></a> [database\_vm\_storage\_nic\_ips](#input\_database\_vm\_storage\_nic\_ips) | If provided, the database tier will be configured with the specified IPs (srorage subnet) | `any` | n/a | yes |
| <a name="input_db_asg_id"></a> [db\_asg\_id](#input\_db\_asg\_id) | Database Application Security Group | `any` | n/a | yes |
| <a name="input_db_subnet"></a> [db\_subnet](#input\_db\_subnet) | Information about SAP db subnet | `any` | n/a | yes |
| <a name="input_deploy_application_security_groups"></a> [deploy\_application\_security\_groups](#input\_deploy\_application\_security\_groups) | Defines if application security groups should be deployed | `any` | n/a | yes |
| <a name="input_deployment"></a> [deployment](#input\_deployment) | The type of deployment | `any` | n/a | yes |
| <a name="input_fencing_role_name"></a> [fencing\_role\_name](#input\_fencing\_role\_name) | If specified the role name to use for the fencing | `any` | n/a | yes |
| <a name="input_hana_ANF_volumes"></a> [hana\_ANF\_volumes](#input\_hana\_ANF\_volumes) | Defines HANA ANF volumes | `any` | n/a | yes |
| <a name="input_infrastructure"></a> [infrastructure](#input\_infrastructure) | n/a | `any` | n/a | yes |
| <a name="input_landscape_tfstate"></a> [landscape\_tfstate](#input\_landscape\_tfstate) | Landscape remote tfstate file | `any` | n/a | yes |
| <a name="input_license_type"></a> [license\_type](#input\_license\_type) | Specifies the license type for the OS | `string` | `""` | no |
| <a name="input_management_dns_resourcegroup_name"></a> [management\_dns\_resourcegroup\_name](#input\_management\_dns\_resourcegroup\_name) | String value giving the possibility to register custom dns a records in a separate resourcegroup | `string` | `null` | no |
| <a name="input_management_dns_subscription_id"></a> [management\_dns\_subscription\_id](#input\_management\_dns\_subscription\_id) | String value giving the possibility to register custom dns a records in a separate subscription | `string` | `null` | no |
| <a name="input_naming"></a> [naming](#input\_naming) | Defines the names for the resources | `any` | n/a | yes |
| <a name="input_options"></a> [options](#input\_options) | n/a | `any` | n/a | yes |
| <a name="input_ppg"></a> [ppg](#input\_ppg) | Details of the proximity placement group | `any` | n/a | yes |
| <a name="input_register_endpoints_with_dns"></a> [register\_endpoints\_with\_dns](#input\_register\_endpoints\_with\_dns) | Boolean value indicating if endpoints should be registered to the dns zone | `bool` | n/a | yes |
| <a name="input_register_virtual_network_to_dns"></a> [register\_virtual\_network\_to\_dns](#input\_register\_virtual\_network\_to\_dns) | Boolean value indicating if the vnet should be registered to the dns zone | `bool` | n/a | yes |
| <a name="input_resource_group"></a> [resource\_group](#input\_resource\_group) | Details of the resource group | `any` | n/a | yes |
| <a name="input_sap_sid"></a> [sap\_sid](#input\_sap\_sid) | The SID of the application | `any` | n/a | yes |
| <a name="input_scale_set_id"></a> [scale\_set\_id](#input\_scale\_set\_id) | Azure resource identifier for scale set | `any` | n/a | yes |
| <a name="input_sdu_public_key"></a> [sdu\_public\_key](#input\_sdu\_public\_key) | Public key used for authentication | `any` | n/a | yes |
| <a name="input_sid_keyvault_user_id"></a> [sid\_keyvault\_user\_id](#input\_sid\_keyvault\_user\_id) | Details of the user keyvault for sap\_system | `any` | n/a | yes |
| <a name="input_sid_password"></a> [sid\_password](#input\_sid\_password) | SDU password | `any` | n/a | yes |
| <a name="input_sid_username"></a> [sid\_username](#input\_sid\_username) | SDU username | `any` | n/a | yes |
| <a name="input_storage_bootdiag_endpoint"></a> [storage\_bootdiag\_endpoint](#input\_storage\_bootdiag\_endpoint) | Details of the boot diagnostics storage account | `any` | n/a | yes |
| <a name="input_storage_subnet"></a> [storage\_subnet](#input\_storage\_subnet) | Information about storage subnet | `any` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | If provided, tags for all resources | `any` | n/a | yes |
| <a name="input_terraform_template_version"></a> [terraform\_template\_version](#input\_terraform\_template\_version) | The version of Terraform templates that were identified in the state file | `any` | n/a | yes |
| <a name="input_use_custom_dns_a_registration"></a> [use\_custom\_dns\_a\_registration](#input\_use\_custom\_dns\_a\_registration) | Boolean value indicating if a custom dns a record should be created when using private endpoints | `bool` | `false` | no |
| <a name="input_use_loadbalancers_for_standalone_deployments"></a> [use\_loadbalancers\_for\_standalone\_deployments](#input\_use\_loadbalancers\_for\_standalone\_deployments) | Defines if load balancers are used even for standalone deployments | `bool` | `true` | no |
| <a name="input_use_msi_for_clusters"></a> [use\_msi\_for\_clusters](#input\_use\_msi\_for\_clusters) | If true, the Pacemaker cluser will use a managed identity | `any` | n/a | yes |
| <a name="input_use_scalesets_for_deployment"></a> [use\_scalesets\_for\_deployment](#input\_use\_scalesets\_for\_deployment) | Use Flexible Virtual Machine Scale Sets for the deployment | `any` | n/a | yes |
| <a name="input_use_secondary_ips"></a> [use\_secondary\_ips](#input\_use\_secondary\_ips) | Use secondary IPs for the SAP System | `bool` | `false` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_ANF_subnet_prefix"></a> [ANF\_subnet\_prefix](#output\_ANF\_subnet\_prefix) | ANF subnet prefix |
| <a name="output_application_volume_group"></a> [application\_volume\_group](#output\_application\_volume\_group) | Application volume group |
| <a name="output_database_disks"></a> [database\_disks](#output\_database\_disks) | Disks used by the database tier |
| <a name="output_database_kdump_disks"></a> [database\_kdump\_disks](#output\_database\_kdump\_disks) | List of Azure disks for kdump |
| <a name="output_database_loadbalancer_id"></a> [database\_loadbalancer\_id](#output\_database\_loadbalancer\_id) | Database loadbalancer Id information |
| <a name="output_database_loadbalancer_ip"></a> [database\_loadbalancer\_ip](#output\_database\_loadbalancer\_ip) | Database loadbalancer IP information |
| <a name="output_database_server_ips"></a> [database\_server\_ips](#output\_database\_server\_ips) | Database Server IP information |
| <a name="output_database_server_secondary_ips"></a> [database\_server\_secondary\_ips](#output\_database\_server\_secondary\_ips) | Database Server IP information |
| <a name="output_database_server_vm_names"></a> [database\_server\_vm\_names](#output\_database\_server\_vm\_names) | HANA Virtual machine names |
| <a name="output_database_shared_disks"></a> [database\_shared\_disks](#output\_database\_shared\_disks) | List of Azure shared disks |
| <a name="output_db_admin_ip"></a> [db\_admin\_ip](#output\_db\_admin\_ip) | Database Admin IP information |
| <a name="output_dns_info_loadbalancers"></a> [dns\_info\_loadbalancers](#output\_dns\_info\_loadbalancers) | Database loadbalancer DNS information |
| <a name="output_dns_info_vms"></a> [dns\_info\_vms](#output\_dns\_info\_vms) | Database server DNS information |
| <a name="output_hana_data_ANF_volumes"></a> [hana\_data\_ANF\_volumes](#output\_hana\_data\_ANF\_volumes) | HANA Data volumes |
| <a name="output_hana_log_ANF_volumes"></a> [hana\_log\_ANF\_volumes](#output\_hana\_log\_ANF\_volumes) | HANA Log volumes |
| <a name="output_hana_shared"></a> [hana\_shared](#output\_hana\_shared) | HANA Shared primary volume |
| <a name="output_hanadb_vm_ids"></a> [hanadb\_vm\_ids](#output\_hanadb\_vm\_ids) | Database loadbalancer DNS information |
| <a name="output_hdb_sid"></a> [hdb\_sid](#output\_hdb\_sid) | Database SID |
| <a name="output_loadbalancers"></a> [loadbalancers](#output\_loadbalancers) | List of disks used in the application tier |
<!-- END_TF_DOCS -->