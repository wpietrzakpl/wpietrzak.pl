---
title: Get-GlpiToolsDropdownsNetworks
---

## SYNOPSIS
Function is getting Network informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworks [-All] [<CommonParameters>]
```

### NetworkId
```
Get-GlpiToolsDropdownsNetworks -NetworkId <String[]> [-Raw] [<CommonParameters>]
```

### NetworkName
```
Get-GlpiToolsDropdownsNetworks -NetworkName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkID which you can find in GLPI website
Returns object with property's of Network

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworks -All
```

Example will return all Network from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworks
```

Function gets NetworkId from GLPI from Pipline, and return Network object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworks
```

Function gets NetworkId from GLPI from Pipline (u can pass many ID's like that), and return Network object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworks -NetworkId 326
```

Function gets NetworkId from GLPI which is provided through -NetworkId after Function type, and return Network object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworks -NetworkId 326, 321
```

Function gets NetworkId from GLPI which is provided through -NetworkId keyword after Function type (u can provide many ID's like that), and return Network object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworks -NetworkName Fusion
```

Example will return glpi Network, but what is the most important, Network will be shown exactly as you see in glpi dropdown Network.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Network from GLPI

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

### -NetworkId
This parameter can take pipline input, either, you can use this function with -NetworkId keyword.
Provide to this param Network ID from GLPI Network Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkId
Aliases: NID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkId Parameter.
NetworkId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkName
This parameter can take pipline input, either, you can use this function with -NetworkName keyword.
Provide to this param Network Name from GLPI Network Bookmark

```yaml
Type: String
Parameter Sets: NetworkName
Aliases: NN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Network ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Network from GLPI
## NOTES
PSP 06/2019

## RELATED LINKS
