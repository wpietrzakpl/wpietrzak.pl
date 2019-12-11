---
title: Get-GlpiToolsDropdownsNetworkEquipmentModels
---

## SYNOPSIS
Function is getting Network Equipment Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworkEquipmentModels [-All] [<CommonParameters>]
```

### NetworkEquipmentModelId
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -NetworkEquipmentModelId <String[]> [-Raw] [<CommonParameters>]
```

### NetworkEquipmentModelName
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -NetworkEquipmentModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkEquipmentModelId which you can find in GLPI website
Returns object with property's of Network Equipment Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -All
```

Example will return all Network Equipment Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworkEquipmentModels
```

Function gets NetworkEquipmentModelId from GLPI from Pipline, and return Network Equipment Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworkEquipmentModels
```

Function gets NetworkEquipmentModelId from GLPI from Pipline (u can pass many ID's like that), and return Network Equipment Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -NetworkEquipmentModelId 326
```

Function gets NetworkEquipmentModelId from GLPI which is provided through -NetworkEquipmentModelId after Function type, and return Network Equipment Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -NetworkEquipmentModelId 326, 321
```

Function gets Network Equipment Models Id from GLPI which is provided through -NetworkEquipmentModelId keyword after Function type (u can provide many ID's like that), and return Network Equipment Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworkEquipmentModels -NetworkEquipmentModelName Fusion
```

Example will return glpi Network Equipment Models, but what is the most important, Network Equipment Models will be shown exactly as you see in glpi dropdown Network Equipment Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Network Equipment Models from GLPI

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

### -NetworkEquipmentModelId
This parameter can take pipline input, either, you can use this function with -NetworkEquipmentModelId keyword.
Provide to this param NetworkEquipmentModelId from GLPI Network Equipment Models Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkEquipmentModelId
Aliases: NEMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkEquipmentModelId Parameter.
NetworkEquipmentModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkEquipmentModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkEquipmentModelName
This parameter can take pipline input, either, you can use this function with -NetworkEquipmentModelId keyword.
Provide to this param Network Equipment Models Name from GLPI Network Equipment Models Bookmark

```yaml
Type: String
Parameter Sets: NetworkEquipmentModelName
Aliases: NEMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Network Equipment Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Network Equipment Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
