---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
---

# New-AzureRmApplicationGatewayBackendAddressPool

## SYNOPSIS
Creates a back-end address pool for an application gateway.

## SYNTAX

### SetByResourceId
```
New-AzureRmApplicationGatewayBackendAddressPool -Name <String>
 [-BackendIPConfigurationIds <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

### SetByIP
```
New-AzureRmApplicationGatewayBackendAddressPool -Name <String>
 [-BackendIPAddresses <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

### SetByFqdn
```
New-AzureRmApplicationGatewayBackendAddressPool -Name <String>
 [-BackendFqdns <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

## DESCRIPTION
The New-AzureRmApplicationGatewayBackendAddressPool cmdlet creates a back-end address pool for an Azure application gateway.
A back-end address can be specified as an IP address, a fully-qualified domain name (FQDN) or an IP configuration ID.

## EXAMPLES

### --------------------------  Example 1: Create a backend address pool by using the FQDN of a backend server  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\>$Pool = New-AzureRmApplicationGatewayBackendAddressPool -Name "Pool01" -BackendFqdns "contoso1.com", "contoso2.com"
```

This command creates a back-end address pool named Pool01 by using the FQDNs of back-end servers, and stores it in the $Pool variable.

### --------------------------  Example 2: Create a backend address pool by using the IP address of a backend server  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\>$Pool = New-AzureRmApplicationGatewayBackendAddressPool -Name "Pool02" -BackendFqdns "10.10.10.10", "10.10.10.11"
```

This command creates a back-end address pool named Pool02 by using the IP addresses of back-end servers, and stores it in the $Pool variable.

## PARAMETERS

### -Name
Specifies the name of the back-end server pool that this cmdlet creates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackendIPConfigurationIds
Specifies a list of back-end server IP configuration IDs that this cmdlet associates with the back-end server pool.```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: SetByResourceId
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackendIPAddresses
Specifies a list of back-end IP addresses that this cmdlet associates with the back-end server pool.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: SetByIP
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BackendFqdns
Specifies a list of back-end FQDNs that this cmdlet associates with the back-end server pool.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: SetByFqdn
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayBackendAddressPool

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayBackendAddressPool]()

[Get-AzureRmApplicationGatewayBackendAddressPool]()

[Remove-AzureRmApplicationGatewayBackendAddressPool]()

[Set-AzureRmApplicationGatewayBackendAddressPool]()

