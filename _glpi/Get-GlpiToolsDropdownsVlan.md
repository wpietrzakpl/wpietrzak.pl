---
title: Get-GlpiToolsDropdownsVlan
---

## SYNOPSIS
Function is getting Vlan informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsVlan [-All] [<CommonParameters>]
```

### VlanId
```
Get-GlpiToolsDropdownsVlan -VlanId <String[]> [-Raw] [<CommonParameters>]
```

### VlanName
```
Get-GlpiToolsDropdownsVlan -VlanName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on VlanId which you can find in GLPI website
Returns object with property's of Vlan

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsVlan -All
```

Example will return all Vlan from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsVlan
```

Function gets VlanId from GLPI from pipeline, and return Vlan object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsVlan
```

Function gets VlanId from GLPI from pipeline (u can pass many ID's like that), and return Vlan object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsVlan -VlanId 326
```

Function gets VlanId from GLPI which is provided through -VlanId after Function type, and return Vlan object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsVlan -VlanId 326, 321
```

Function gets Vlan Id from GLPI which is provided through -VlanId keyword after Function type (u can provide many ID's like that), and return Vlan object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsVlan -VlanName Fusion
```

Example will return glpi Vlan, but what is the most important, Vlan will be shown exactly as you see in glpi dropdown Vlan.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Vlan from GLPI

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

### -VlanId
This parameter can take pipeline input, either, you can use this function with -VlanId keyword.
Provide to this param VlanId from GLPI Vlan Bookmark

```yaml
Type: String[]
Parameter Sets: VlanId
Aliases: VID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with VlanId Parameter.
VlanId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: VlanId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -VlanName
This parameter can take pipeline input, either, you can use this function with -VlanId keyword.
Provide to this param Vlan Name from GLPI Vlan Bookmark

```yaml
Type: String
Parameter Sets: VlanName
Aliases: VN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Vlan ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Vlan from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
