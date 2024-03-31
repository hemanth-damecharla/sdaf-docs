<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | ~> 3.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_azurerm"></a> [azurerm](#provider\_azurerm) | ~> 3.0 |
| <a name="provider_azurerm.deployer"></a> [azurerm.deployer](#provider\_azurerm.deployer) | ~> 3.0 |
| <a name="provider_azurerm.dnsmanagement"></a> [azurerm.dnsmanagement](#provider\_azurerm.dnsmanagement) | ~> 3.0 |
| <a name="provider_azurerm.main"></a> [azurerm.main](#provider\_azurerm.main) | ~> 3.0 |
| <a name="provider_random"></a> [random](#provider\_random) | n/a |
| <a name="provider_time"></a> [time](#provider\_time) | n/a |

## Modules

sap_library.

## Resources

| Name | Type |
|------|------|
| [azurerm_key_vault_secret.sa_connection_string](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/key_vault_secret) | resource |
| [azurerm_key_vault_secret.sapbits_location_base_path](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/key_vault_secret) | resource |
| [azurerm_key_vault_secret.saplibrary_access_key](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/key_vault_secret) | resource |
| [azurerm_key_vault_secret.tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/key_vault_secret) | resource |
| [azurerm_management_lock.storage_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/management_lock) | resource |
| [azurerm_private_dns_a_record.kv_user](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_a_record) | resource |
| [azurerm_private_dns_a_record.storage_sapbits_pep_a_record_registry](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_a_record) | resource |
| [azurerm_private_dns_a_record.storage_tfstate_pep_a_record_registry](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_a_record) | resource |
| [azurerm_private_dns_zone.blob](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone) | resource |
| [azurerm_private_dns_zone.dns](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone) | resource |
| [azurerm_private_dns_zone.file](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone) | resource |
| [azurerm_private_dns_zone.table](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone) | resource |
| [azurerm_private_dns_zone.vault](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone) | resource |
| [azurerm_private_dns_zone_virtual_network_link.vault](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone_virtual_network_link) | resource |
| [azurerm_private_dns_zone_virtual_network_link.vnet_mgmt](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone_virtual_network_link) | resource |
| [azurerm_private_dns_zone_virtual_network_link.vnet_mgmt_blob](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_dns_zone_virtual_network_link) | resource |
| [azurerm_private_endpoint.kv_user](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_endpoint) | resource |
| [azurerm_private_endpoint.storage_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_endpoint) | resource |
| [azurerm_private_endpoint.storage_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_endpoint) | resource |
| [azurerm_private_endpoint.table_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/private_endpoint) | resource |
| [azurerm_resource_group.library](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group) | resource |
| [azurerm_role_assignment.storage_sapbits_contributor](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_role_assignment.storage_sapbits_contributor_ssi](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_role_assignment.storage_tfstate_contributor](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_role_assignment.storage_tfstate_contributor_ssi](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/role_assignment) | resource |
| [azurerm_storage_account.storage_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_account) | resource |
| [azurerm_storage_account.storage_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_account) | resource |
| [azurerm_storage_container.storagecontainer_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_container) | resource |
| [azurerm_storage_container.storagecontainer_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_container) | resource |
| [azurerm_storage_container.storagecontainer_tfvars](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_container) | resource |
| [azurerm_storage_share.fileshare_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/storage_share) | resource |
| [random_id.post_fix](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/id) | resource |
| [time_offset.secret_expiry_date](https://registry.terraform.io/providers/hashicorp/time/latest/docs/resources/offset) | resource |
| [time_sleep.wait_for_dns_refresh](https://registry.terraform.io/providers/hashicorp/time/latest/docs/resources/sleep) | resource |
| [azurerm_network_interface.storage_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/network_interface) | data source |
| [azurerm_network_interface.storage_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/network_interface) | data source |
| [azurerm_private_dns_zone.storage](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/private_dns_zone) | data source |
| [azurerm_private_dns_zone.table](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/private_dns_zone) | data source |
| [azurerm_private_dns_zone.vault](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/private_dns_zone) | data source |
| [azurerm_resource_group.library](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/resource_group) | data source |
| [azurerm_storage_account.storage_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/storage_account) | data source |
| [azurerm_storage_account.storage_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/storage_account) | data source |
| [azurerm_storage_container.storagecontainer_sapbits](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/storage_container) | data source |
| [azurerm_storage_container.storagecontainer_tfstate](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/storage_container) | data source |
| [azurerm_storage_container.storagecontainer_tfvars](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/storage_container) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_Agent_IP"></a> [Agent\_IP](#input\_Agent\_IP) | If provided, contains the IP address of the agent | `string` | `""` | no |
| <a name="input_bootstrap"></a> [bootstrap](#input\_bootstrap) | n/a | `any` | n/a | yes |
| <a name="input_deployer"></a> [deployer](#input\_deployer) | Details of deployer | `map` | `{}` | no |
| <a name="input_deployer_tfstate"></a> [deployer\_tfstate](#input\_deployer\_tfstate) | terraform.tfstate of deployer | `map` | `{}` | no |
| <a name="input_dns_label"></a> [dns\_label](#input\_dns\_label) | DNS label for the deployment | `string` | `""` | no |
| <a name="input_dns_zone_names"></a> [dns\_zone\_names](#input\_dns\_zone\_names) | Private DNS zone names | `map(string)` | <pre>{<br>  "blob_dns_zone_name": "privatelink.blob.core.windows.net",<br>  "file_dns_zone_name": "privatelink.file.core.windows.net",<br>  "table_dns_zone_name": "privatelink.table.core.windows.net",<br>  "vault_dns_zone_name": "privatelink.vaultcore.azure.net"<br>}</pre> | no |
| <a name="input_enable_purge_control_for_keyvaults"></a> [enable\_purge\_control\_for\_keyvaults](#input\_enable\_purge\_control\_for\_keyvaults) | Allow the deployment to control the purge protection | `bool` | `true` | no |
| <a name="input_infrastructure"></a> [infrastructure](#input\_infrastructure) | Details of the Azure infrastructure to deploy the SAP library into | `map` | `{}` | no |
| <a name="input_key_vault"></a> [key\_vault](#input\_key\_vault) | Import existing Azure Key Vaults | `map` | `{}` | no |
| <a name="input_management_dns_resourcegroup_name"></a> [management\_dns\_resourcegroup\_name](#input\_management\_dns\_resourcegroup\_name) | String value giving the possibility to register custom dns a records in a separate resourcegroup | `string` | `null` | no |
| <a name="input_management_dns_subscription_id"></a> [management\_dns\_subscription\_id](#input\_management\_dns\_subscription\_id) | String value giving the possibility to register custom dns a records in a separate subscription | `string` | `null` | no |
| <a name="input_naming"></a> [naming](#input\_naming) | naming convention data structure | `any` | n/a | yes |
| <a name="input_place_delete_lock_on_resources"></a> [place\_delete\_lock\_on\_resources](#input\_place\_delete\_lock\_on\_resources) | If defined, a delete lock will be placed on the key resources | `any` | n/a | yes |
| <a name="input_service_principal"></a> [service\_principal](#input\_service\_principal) | Current service principal used to authenticate to Azure | `any` | n/a | yes |
| <a name="input_short_named_endpoints_nics"></a> [short\_named\_endpoints\_nics](#input\_short\_named\_endpoints\_nics) | If defined, uses short names for private endpoints nics | `bool` | `false` | no |
| <a name="input_storage_account_sapbits"></a> [storage\_account\_sapbits](#input\_storage\_account\_sapbits) | n/a | `any` | n/a | yes |
| <a name="input_storage_account_tfstate"></a> [storage\_account\_tfstate](#input\_storage\_account\_tfstate) | n/a | `any` | n/a | yes |
| <a name="input_use_custom_dns_a_registration"></a> [use\_custom\_dns\_a\_registration](#input\_use\_custom\_dns\_a\_registration) | Boolean value indicating if a custom dns a record should be created when using private endpoints | `bool` | `false` | no |
| <a name="input_use_private_endpoint"></a> [use\_private\_endpoint](#input\_use\_private\_endpoint) | Boolean value indicating if private endpoint should be used for the deployment | `bool` | `false` | no |
| <a name="input_use_webapp"></a> [use\_webapp](#input\_use\_webapp) | n/a | `bool` | `false` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_created_resource_group_id"></a> [created\_resource\_group\_id](#output\_created\_resource\_group\_id) | Created resource group ID |
| <a name="output_created_resource_group_name"></a> [created\_resource\_group\_name](#output\_created\_resource\_group\_name) | Created resource group name |
| <a name="output_created_resource_group_subscription_id"></a> [created\_resource\_group\_subscription\_id](#output\_created\_resource\_group\_subscription\_id) | Created resource group' subscription ID |
| <a name="output_random_id"></a> [random\_id](#output\_random\_id) | n/a |
| <a name="output_random_id_b64"></a> [random\_id\_b64](#output\_random\_id\_b64) | n/a |
| <a name="output_remote_state_storage_account_name"></a> [remote\_state\_storage\_account\_name](#output\_remote\_state\_storage\_account\_name) | Storage account name for Terraform remote state |
| <a name="output_sa_connection_string"></a> [sa\_connection\_string](#output\_sa\_connection\_string) | Connection string to storage account |
| <a name="output_sapbits_sa_resource_group_name"></a> [sapbits\_sa\_resource\_group\_name](#output\_sapbits\_sa\_resource\_group\_name) | SAPBits storage account resource group name |
| <a name="output_sapbits_storage_account_name"></a> [sapbits\_storage\_account\_name](#output\_sapbits\_storage\_account\_name) | SAPBits storage account name |
| <a name="output_storagecontainer_sapbits_name"></a> [storagecontainer\_sapbits\_name](#output\_storagecontainer\_sapbits\_name) | SAP Bits container name |
| <a name="output_storagecontainer_tfstate"></a> [storagecontainer\_tfstate](#output\_storagecontainer\_tfstate) | TFState container name |
| <a name="output_tfstate_resource_id"></a> [tfstate\_resource\_id](#output\_tfstate\_resource\_id) | value of the Azure resource id for the tfstate storage account |
| <a name="output_tfstate_storage_account"></a> [tfstate\_storage\_account](#output\_tfstate\_storage\_account) | TFState storage account name |
<!-- END_TF_DOCS -->