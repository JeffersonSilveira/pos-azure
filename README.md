# pos-azure
Aqui está os arquivos json gerados no projeto final do módulo Azure
## Grupo de recursos
```
{
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex",
    "name": "rg-clientex",
    "type": "Microsoft.Resources/resourceGroups",
    "location": "brazilsouth",
    "tags": {},
    "properties": {
        "provisioningState": "Succeeded"
    }
}
```
## Application gateway

```
{
    "name": "appGw-clientex",
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex",
    "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
    "type": "Microsoft.Network/applicationGateways",
    "location": "brazilsouth",
    "tags": {},
    "properties": {
        "provisioningState": "Succeeded",
        "resourceGuid": "0104b9de-0f08-40e2-861a-d659eb69548e",
        "sku": {
            "name": "Standard_v2",
            "tier": "Standard_v2"
        },
        "operationalState": "Running",
        "gatewayIPConfigurations": [
            {
                "name": "appGatewayIpConfig",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/gatewayIPConfigurations/appGatewayIpConfig",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "subnet": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/virtualNetworks/appGw-clientex/subnets/sNappGw-clientex"
                    }
                },
                "type": "Microsoft.Network/applicationGateways/gatewayIPConfigurations"
            }
        ],
        "sslCertificates": [],
        "frontendIPConfigurations": [
            {
                "name": "appGwPublicFrontendIpIPv4",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/frontendIPConfigurations/appGwPublicFrontendIpIPv4",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "type": "Microsoft.Network/applicationGateways/frontendIPConfigurations",
                "properties": {
                    "provisioningState": "Succeeded",
                    "privateIPAllocationMethod": "Dynamic",
                    "publicIPAddress": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/publicIPAddresses/PIP-appGw-clientex"
                    },
                    "httpListeners": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/httpListeners/l-appGw-clientex"
                        }
                    ]
                }
            }
        ],
        "frontendPorts": [
            {
                "name": "port_80",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/frontendPorts/port_80",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "port": 80,
                    "httpListeners": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/httpListeners/l-appGw-clientex"
                        }
                    ]
                },
                "type": "Microsoft.Network/applicationGateways/frontendPorts"
            }
        ],
        "backendAddressPools": [
            {
                "name": "Backend-appGw-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/backendAddressPools/Backend-appGw-clientex",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "backendIPConfigurations": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Compute/virtualMachineScaleSets/vmss-clientex/virtualMachines/0/networkInterfaces/appGw-clientex-nic01/ipConfigurations/appGw-clientex-nic01-defaultIpConfiguration"
                        }
                    ],
                    "backendAddresses": [],
                    "requestRoutingRules": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/requestRoutingRules/r-appGw-clientex"
                        }
                    ]
                },
                "type": "Microsoft.Network/applicationGateways/backendAddressPools"
            }
        ],
        "backendHttpSettingsCollection": [
            {
                "name": "HTTPConfig-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvdfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/backendHttpSettingsCollection/HTTPConfig-clientex",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "port": 80,
                    "protocol": "Http",
                    "cookieBasedAffinity": "Disabled",
                    "pickHostNameFromBackendAddress": false,
                    "requestTimeout": 20,
                    "requestRoutingRules": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/requestRoutingRules/r-appGw-clientex"
                        }
                    ]
                },
                "type": "Microsoft.Network/applicationGateways/backendHttpSettingsCollection"
            }
        ],
        "httpListeners": [
            {
                "name": "l-appGw-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/httpListeners/l-appGw-clientex",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "frontendIPConfiguration": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/frontendIPConfigurations/appGwPublicFrontendIpIPv4"
                    },
                    "frontendPort": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/frontendPorts/port_80"
                    },
                    "protocol": "Http",
                    "requireServerNameIndication": false,
                    "requestRoutingRules": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/requestRoutingRules/r-appGw-clientex"
                        }
                    ]
                },
                "type": "Microsoft.Network/applicationGateways/httpListeners"
            }
        ],
        "urlPathMaps": [],
        "requestRoutingRules": [
            {
                "name": "r-appGw-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/requestRoutingRules/r-appGw-clientex",
                "etag": "W/\"487f4ec1-55db-44d5-965d-c1bb7e8a5969\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "ruleType": "Basic",
                    "httpListener": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/httpListeners/l-appGw-clientex"
                    },
                    "backendAddressPool": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/backendAddressPools/Backend-appGw-clientex"
                    },
                    "backendHttpSettings": {
                        "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/backendHttpSettingsCollection/HTTPConfig-clientex"
                    }
                },
                "type": "Microsoft.Network/applicationGateways/requestRoutingRules"
            }
        ],
        "probes": [],
        "redirectConfigurations": [],
        "enableHttp2": false
    }
}
```

## Rede virtual
```
{
    "name": "appGw-clientex",
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/virtualNetworks/appGw-clientex",
    "etag": "W/\"5fa8ded2-1494-40b6-ad01-7e56caef8c0b\"",
    "type": "Microsoft.Network/virtualNetworks",
    "location": "brazilsouth",
    "tags": {},
    "properties": {
        "provisioningState": "Succeeded",
        "resourceGuid": "94f810bc-96b0-4e99-82c4-f5cesda23b672bd3f",
        "addressSpace": {
            "addressPrefixes": [
                "10.0.0.0/16"
            ]
        },
        "subnets": [
            {
                "name": "sNappGw-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/virtualNetworks/appGw-clientex/subnets/sNappGw-clientex",
                "etag": "W/\"5fa8ded2-1494-40b6-ad01-7e56caef8c0b\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "addressPrefix": "10.0.0.0/24",
                    "applicationGatewayIPConfigurations": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/gatewayIPConfigurations/appGatewayIpConfig"
                        }
                    ]
                },
                "type": "Microsoft.Network/virtualNetworks/subnets"
            },
            {
                "name": "sNVMSS-clientex",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/virtualNetworks/appGw-clientex/subnets/sNVMSS-clientex",
                "etag": "W/\"5fa8ded2-1494-40b6-ad01-7e56caef8c0b\"",
                "properties": {
                    "provisioningState": "Succeeded",
                    "addressPrefix": "10.0.1.0/24",
                    "ipConfigurations": [
                        {
                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Compute/virtualMachineScaleSets/vmss-clientex/virtualMachines/0/networkInterfaces/appGw-clientex-nic01/ipConfigurations/appGw-clientex-nic01-defaultIpConfiguration"
                        }
                    ]
                },
                "type": "Microsoft.Network/virtualNetworks/subnets"
            }
        ]
    }
}
```

## Grupo de segurança de rede
```
{
    "name": "basicNsgappGw-clientex-nic01",
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01",
    "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
    "type": "Microsoft.Network/networkSecurityGroups",
    "location": "brazilsouth",
    "properties": {
        "provisioningState": "Succeeded",
        "resourceGuid": "cef7577b-a135-4da0-a2e4-b8f15b3ad789",
        "securityRules": [],
        "defaultSecurityRules": [
            {
                "name": "AllowVnetInBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/AllowVnetInBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Allow inbound traffic from all VMs in VNET",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "VirtualNetwork",
                    "destinationAddressPrefix": "VirtualNetwork",
                    "access": "Allow",
                    "priority": 65000,
                    "direction": "Inbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            },
            {
                "name": "AllowAzureLoadBalancerInBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/AllowAzureLoadBalancerInBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Allow inbound traffic from azure load balancer",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "AzureLoadBalancer",
                    "destinationAddressPrefix": "*",
                    "access": "Allow",
                    "priority": 65001,
                    "direction": "Inbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            },
            {
                "name": "DenyAllInBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/DenyAllInBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Deny all inbound traffic",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "*",
                    "destinationAddressPrefix": "*",
                    "access": "Deny",
                    "priority": 65500,
                    "direction": "Inbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            },
            {
                "name": "AllowVnetOutBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/AllowVnetOutBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Allow outbound traffic from all VMs to all VMs in VNET",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "VirtualNetwork",
                    "destinationAddressPrefix": "VirtualNetwork",
                    "access": "Allow",
                    "priority": 65000,
                    "direction": "Outbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            },
            {
                "name": "AllowInternetOutBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/AllowInternetOutBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Allow outbound traffic from all VMs to Internet",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "*",
                    "destinationAddressPrefix": "Internet",
                    "access": "Allow",
                    "priority": 65001,
                    "direction": "Outbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            },
            {
                "name": "DenyAllOutBound",
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01/defaultSecurityRules/DenyAllOutBound",
                "etag": "W/\"2851693b-36f6-4d39-9275-8b089e0b64fc\"",
                "type": "Microsoft.Network/networkSecurityGroups/defaultSecurityRules",
                "properties": {
                    "provisioningState": "Succeeded",
                    "description": "Deny all outbound traffic",
                    "protocol": "*",
                    "sourcePortRange": "*",
                    "destinationPortRange": "*",
                    "sourceAddressPrefix": "*",
                    "destinationAddressPrefix": "*",
                    "access": "Deny",
                    "priority": 65500,
                    "direction": "Outbound",
                    "sourcePortRanges": [],
                    "destinationPortRanges": [],
                    "sourceAddressPrefixes": [],
                    "destinationAddressPrefixes": []
                }
            }
        ],
        "networkInterfaces": [
            {
                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Compute/virtualMachineScaleSets/vmss-clientex/virtualMachines/0/networkInterfaces/appGw-clientex-nic01"
            }
        ]
    }
}
```

## Endereço IP público
```
{
    "name": "PIP-appGw-clientex",
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/publicIPAddresses/PIP-appGw-clientex",
    "etag": "W/\"0b3bc6e1-4bff-47f9-bc4d-3365aabcf5a8\"",
    "location": "brazilsouth",
    "properties": {
        "provisioningState": "Succeeded",
        "resourceGuid": "6c66fe6f-a3f9-4b02-b3f1-11849775b65f",
        "ipAddress": "20.226.24.116",
        "publicIPAddressVersion": "IPv4",
        "publicIPAllocationMethod": "Static",
        "idleTimeoutInMinutes": 4,
        "ipTags": [],
        "ipConfiguration": {
            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/frontendIPConfigurations/appGwPublicFrontendIpIPv4"
        }
    },
    "type": "Microsoft.Network/publicIPAddresses",
    "sku": {
        "name": "Standard"
    }
}
```
## Conjunto de escalas da máquina virtual
```
{
    "name": "vmss-clientex",
    "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Compute/virtualMachineScaleSets/vmss-clientex",
    "type": "Microsoft.Compute/virtualMachineScaleSets",
    "location": "brazilsouth",
    "sku": {
        "name": "Standard_B1ls",
        "tier": "Standard",
        "capacity": 1
    },
    "properties": {
        "singlePlacementGroup": false,
        "orchestrationMode": "Uniform",
        "upgradePolicy": {
            "mode": "Manual"
        },
        "scaleInPolicy": {
            "rules": [
                "Default"
            ],
            "forceDeletion": false
        },
        "virtualMachineProfile": {
            "osProfile": {
                "computerNamePrefix": "vmss-clie",
                "adminUsername": "azureuser",
                "linuxConfiguration": {
                    "disablePasswordAuthentication": true,
                    "ssh": {
                        "publicKeys": [
                            {
                                "path": "/home/azureuser/.ssh/authorized_keys",
                                "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgAHYoChQVBUNpwRDm8/rEWJ07N6yBnDh4U/WM27za/3VkpfXqdx2/I0Ki2oB9kU8TNqsh133wnC/hBxX9IHBHi1HGSu8DB++6vunRQyVh7Eta5OD9PAC/8zSNoGOV4z/gWKewTRpm9MW4XVhOb4KWOHE4VzxqEDZSbp1hK75tgvaGRixvFMbXH2H0gKSYs/GhOMr0LQsDwqqM0RzVhUxotS7C1NH8RvFtCbvwY0xSfVRDgs5SOZF+ulpriKLnEm8CIesO1cUQbWVQnuSzMfsElLMgR0wkYhDDKUJluiqJeHA6tCt166HtWWeqtj7k/OUviUKGKLRRAP++Ugj+4aXqSPr8udNezR/Lw1KIho0W4M6WMZpNNReb4gCYd/uxGQQVizG/ovGqSKo16Tgu+HDZQJMNcNm0pN1psyMdmNhoTedxcSHOPQa0bhE= generated-by-azure"
                            }
                        ]
                    },
                    "provisionVMAgent": true,
                    "enableVMAgentPlatformUpdates": false
                },
                "secrets": [],
                "allowExtensionOperations": true,
                "requireGuestProvisionSignal": true
            },
            "storageProfile": {
                "osDisk": {
                    "osType": "Linux",
                    "createOption": "FromImage",
                    "caching": "ReadWrite",
                    "managedDisk": {
                        "storageAccountType": "Premium_LRS"
                    },
                    "diskSizeGB": 30
                },
                "imageReference": {
                    "publisher": "canonical",
                    "offer": "0001-com-ubuntu-server-focal",
                    "sku": "20_04-lts-gen2",
                    "version": "latest"
                },
                "diskControllerType": "SCSI"
            },
            "networkProfile": {
                "networkInterfaceConfigurations": [
                    {
                        "name": "appGw-clientex-nic01",
                        "properties": {
                            "primary": true,
                            "enableAcceleratedNetworking": false,
                            "disableTcpStateTracking": false,
                            "networkSecurityGroup": {
                                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/networkSecurityGroups/basicNsgappGw-clientex-nic01"
                            },
                            "dnsSettings": {
                                "dnsServers": []
                            },
                            "enableIPForwarding": false,
                            "ipConfigurations": [
                                {
                                    "name": "appGw-clientex-nic01-defaultIpConfiguration",
                                    "properties": {
                                        "primary": true,
                                        "subnet": {
                                            "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/virtualNetworks/appGw-clientex/subnets/sNVMSS-clientex"
                                        },
                                        "privateIPAddressVersion": "IPv4",
                                        "applicationGatewayBackendAddressPools": [
                                            {
                                                "id": "/subscriptions/043271fb-c2ab-4477-940c-4495df3a30edfcvd/resourceGroups/rg-clientex/providers/Microsoft.Network/applicationGateways/appGw-clientex/backendAddressPools/Backend-appGw-clientex"
                                            }
                                        ]
                                    }
                                }
                            ]
                        }
                    }
                ]
            },
            "diagnosticsProfile": {
                "bootDiagnostics": {
                    "enabled": true
                }
            },
            "extensionProfile": {
                "extensions": []
            }
        },
        "provisioningState": "Succeeded",
        "overprovision": false,
        "doNotRunExtensionsOnOverprovisionedVMs": false,
        "uniqueId": "5523340d-90c3-430b-91f6-654072cdf27f",
        "platformFaultDomainCount": 1,
        "timeCreated": "2023-05-27T15:21:03.3431002+00:00"
    }
}
```

