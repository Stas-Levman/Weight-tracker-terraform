# Weight tracker terraform


In this project i built a weight tracker web application using Terraform and Azure as my cloud provider,
Each module in the project has it's own readme with descriptions of the variables and the main.tf files have comments for each resource exaplaining what they do.

**In order to be able to build the infrastruce a custom .rfvars file needs to be used for the apply command**

Instead of a .tfvars file i used azure vault to store and retrieve all my senestive content,
when using a .tfvars the variable `is-azure-vault-enabled` should be set to false, the code will recognize this and will not to try to promt vault for the sensitive data.

If you recived a custom .tfvars file from me, the variable should already be set to false by default and ready to be used to build the infrastructure.

###resources used in the template###

- `azure-vault`
- `azurerm_resource_group`
- `azurerm_virtual_network`
- `azurerm_public_ip`
- `azurerm_network_security_group`
- `azurerm_subnet`
- `azurerm_subnet_network_security_group_association`

- `azurerm_lb`
- `azurerm_lb_backend_address_pool`
- `azurerm_lb_outbound_rule`
- `azurerm_lb_probe`
- `azurerm_lb_rule`
- `azurerm_lb_nat_pool`


- `azurerm_private_dns_zone`
- `azurerm_private_dns_zone_virtual_network_link`
- `azurerm_postgresql_flexible_server`
- `azurerm_postgresql_flexible_server_configuration`

- `azurerm_linux_virtual_machine_scale_set`
- `azurerm_monitor_autoscale_setting`
- `
- `azurerm_network_interface` - not used in the project
- `azurerm_linux_virtual_machine` - not used in the project
###Special provider resources used in the template###
- `http
- `
- `



###Instructions###
Start by installing all the needed packages for this 

