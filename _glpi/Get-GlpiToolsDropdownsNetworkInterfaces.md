---
title: Get-GlpiToolsDropdownsNetworkInterfaces
---

## SYNOPSIS
Function is getting Network Interfaces informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworkInterfaces [-All] [<CommonParameters>]
```

### NetworkInterfaceId
```
Get-GlpiToolsDropdownsNetworkInterfaces -NetworkInterfaceId <String[]> [-Raw] [<CommonParameters>]
```

### NetworkInterfaceName
```
Get-GlpiToolsDropdownsNetworkInterfaces -NetworkInterfaceName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkInterfaceId which you can find in GLPI website
Returns object with property's of Network Interfaces

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworkInterfaces -All
```

Example will return all Network Interfaces from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworkInterfaces
```

Function gets NetworkInterfaceId from GLPI from pipeline, and return Network Interfaces object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworkInterfaces
```

Function gets NetworkInterfaceId from GLPI from pipeline (u can pass many ID's like that), and return Network Interfaces object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworkInterfaces -NetworkInterfaceId 326
```

Function gets NetworkInterfaceId from GLPI which is provided through -NetworkInterfaceId after Function type, and return Network Interfaces object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworkInterfaces -NetworkInterfaceId 326, 321
```

Function gets Network Interfaces Id from GLPI which is provided through -NetworkInterfaceId keyword after Function type (u can provide many ID's like that), and return Network Interfaces object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworkInterfaces -NetworkInterfaceName Fusion
```

Example will return glpi Network Interfaces, but what is the most important, Network Interfaces will be shown exactly as you see in glpi dropdown Network Interfaces.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Network Interfaces from GLPI

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

### -NetworkInterfaceId
This parameter can take pipeline input, either, you can use this function with -NetworkInterfaceId keyword.
Provide to this param NetworkInterfaceId from GLPI Network Interfaces Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkInterfaceId
Aliases: NIID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkInterfaceId Parameter.
NetworkInterfaceId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkInterfaceId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkInterfaceName
This parameter can take pipeline input, either, you can use this function with -NetworkInterfaceId keyword.
Provide to this param Network Interfaces Name from GLPI Network Interfaces Bookmark

```yaml
Type: String
Parameter Sets: NetworkInterfaceName
Aliases: NIN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Network Interfaces ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Network Interfaces from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
