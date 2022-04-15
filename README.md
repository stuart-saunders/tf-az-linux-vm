# Azure Linux VM Module

Usage:-
```
module "linux-vm" {
  source  = "./modules/linux-vm"
  vm_name = "linux-vm"

  ip_configuration_name = var.ip_configuration_name
  subnet_id             = azurerm_subnet.this.id
  location              = azurerm_resource_group.this.location
  resource_group_name   = azurerm_resource_group.this.name
}
```