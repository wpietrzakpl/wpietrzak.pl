---
title: Get-GlpiToolsDropdownsNetworkOutlets
---

## SYNOPSIS
Function is getting Network Outlets informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworkOutlets [-All] [<CommonParameters>]
```

### NetworkOutletId
```
Get-GlpiToolsDropdownsNetworkOutlets -NetworkOutletId <String[]> [-Raw] [<CommonParameters>]
```

### NetworkOutletName
```
Get-GlpiToolsDropdownsNetworkOutlets -NetworkOutletName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkOutletId which you can find in GLPI website
Returns object with property's of Network Outlets

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworkOutlets -All
```

Example will return all Network Outlets from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworkOutlets
```

Function gets NetworkOutletId from GLPI from pipeline, and return Network Outlets object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworkOutlets
```

Function gets NetworkOutletId from GLPI from pipeline (u can pass many ID's like that), and return Network Outlets object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworkOutlets -NetworkOutletId 326
```

Function gets NetworkOutletId from GLPI which is provided through -NetworkOutletId after Function type, and return Network Outlets object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworkOutlets -NetworkOutletId 326, 321
```

Function gets Network Outlets Id from GLPI which is provided through -NetworkOutletId keyword after Function type (u can provide many ID's like that), and return Network Outlets object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworkOutlets -NetworkOutletName Fusion
```

Example will return glpi Network Outlets, but what is the most important, Network Outlets will be shown exactly as you see in glpi dropdown Network Outlets.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Network Outlets from GLPI

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

### -NetworkOutletId
This parameter can take pipeline input, either, you can use this function with -NetworkOutletId keyword.
Provide to this param NetworkOutletId from GLPI Network Outlets Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkOutletId
Aliases: NOID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkOutletId Parameter.
NetworkOutletId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkOutletId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkOutletName
This parameter can take pipeline input, either, you can use this function with -NetworkOutletId keyword.
Provide to this param Network Outlets Name from GLPI Network Outlets Bookmark

```yaml
Type: String
Parameter Sets: NetworkOutletName
Aliases: NON

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Network Outlets ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Network Outlets from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
