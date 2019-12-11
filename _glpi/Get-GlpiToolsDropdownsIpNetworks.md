---
title: Get-GlpiToolsDropdownsIpNetworks
---

## SYNOPSIS
Function is getting Ip Networks informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsIpNetworks [-All] [<CommonParameters>]
```

### IpNetworkId
```
Get-GlpiToolsDropdownsIpNetworks -IpNetworkId <String[]> [-Raw] [<CommonParameters>]
```

### IpNetworkName
```
Get-GlpiToolsDropdownsIpNetworks -IpNetworkName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on IpNetworkId which you can find in GLPI website
Returns object with property's of Ip Networks

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsIpNetworks -All
```

Example will return all Ip Networks from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsIpNetworks
```

Function gets IpNetworkId from GLPI from pipeline, and return Ip Networks object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsIpNetworks
```

Function gets IpNetworkId from GLPI from pipeline (u can pass many ID's like that), and return Ip Networks object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsIpNetworks -IpNetworkId 326
```

Function gets IpNetworkId from GLPI which is provided through -IpNetworkId after Function type, and return Ip Networks object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsIpNetworks -IpNetworkId 326, 321
```

Function gets Ip Networks Id from GLPI which is provided through -IpNetworkId keyword after Function type (u can provide many ID's like that), and return Ip Networks object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsIpNetworks -IpNetworkName Fusion
```

Example will return glpi Ip Networks, but what is the most important, Ip Networks will be shown exactly as you see in glpi dropdown Ip Networks.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Ip Networks from GLPI

```yaml
Type: SwitchParameter
Parameter Sets: All
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IpNetworkId
This parameter can take pipeline input, either, you can use this function with -IpNetworkId keyword.
Provide to this param IpNetworkId from GLPI Ip Networks Bookmark

```yaml
Type: String[]
Parameter Sets: IpNetworkId
Aliases: INID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with IpNetworkId Parameter.
IpNetworkId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: IpNetworkId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IpNetworkName
This parameter can take pipeline input, either, you can use this function with -IpNetworkId keyword.
Provide to this param Ip Networks Name from GLPI Ip Networks Bookmark

```yaml
Type: String
Parameter Sets: IpNetworkName
Aliases: INN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Ip Networks ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Ip Networks from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
