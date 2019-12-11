---
title: Get-GlpiToolsDropdownsNetworkingEquipmentTypes
---

## SYNOPSIS
Function is getting Networking Equipment Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes [-All] [<CommonParameters>]
```

### NetworkingEquipmentTypeId
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -NetworkingEquipmentTypeId <String[]> [-Raw]
 [<CommonParameters>]
```

### NetworkingEquipmentTypeName
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -NetworkingEquipmentTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkingEquipmentTypeId which you can find in GLPI website
Returns object with property's of Networking Equipment Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -All
```

Example will return all Networking Equipment Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworkingEquipmentTypes
```

Function gets NetworkingEquipmentTypeId from GLPI from Pipline, and return Networking Equipment Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworkingEquipmentTypes
```

Function gets NetworkingEquipmentTypeId from GLPI from Pipline (u can pass many ID's like that), and return Networking Equipment Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -NetworkingEquipmentTypeId 326
```

Function gets NetworkingEquipmentTypeId from GLPI which is provided through -NetworkingEquipmentTypeId after Function type, and return Networking Equipment Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -NetworkingEquipmentTypeId 326, 321
```

Function gets Networking Equipment Types Id from GLPI which is provided through -NetworkingEquipmentTypeId keyword after Function type (u can provide many ID's like that), and return Networking Equipment Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworkingEquipmentTypes -NetworkingEquipmentTypeName Fusion
```

Example will return glpi Networking Equipment Types, but what is the most important, Networking Equipment Types will be shown exactly as you see in glpi dropdown Networking Equipment Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Networking Equipment Types from GLPI

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

### -NetworkingEquipmentTypeId
This parameter can take pipline input, either, you can use this function with -NetworkingEquipmentTypeId keyword.
Provide to this param NetworkingEquipmentTypeId from GLPI Networking Equipment Types Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkingEquipmentTypeId
Aliases: NETID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkingEquipmentTypeId Parameter.
NetworkingEquipmentTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkingEquipmentTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkingEquipmentTypeName
This parameter can take pipline input, either, you can use this function with -NetworkingEquipmentTypeId keyword.
Provide to this param Networking Equipment Types Name from GLPI Networking Equipment Types Bookmark

```yaml
Type: String
Parameter Sets: NetworkingEquipmentTypeName
Aliases: NETN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Networking Equipment Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Networking Equipment Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
