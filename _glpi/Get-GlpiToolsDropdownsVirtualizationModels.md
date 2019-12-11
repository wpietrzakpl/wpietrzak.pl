---
title: Get-GlpiToolsDropdownsVirtualizationModels
---

## SYNOPSIS
Function is getting Virtualization Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsVirtualizationModels [-All] [<CommonParameters>]
```

### VirtualizationModelId
```
Get-GlpiToolsDropdownsVirtualizationModels -VirtualizationModelId <String[]> [-Raw] [<CommonParameters>]
```

### VirtualizationModelName
```
Get-GlpiToolsDropdownsVirtualizationModels -VirtualizationModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on VirtualizationModelId which you can find in GLPI website
Returns object with property's of Virtualization Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsVirtualizationModels -All
```

Example will return all Virtualization Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsVirtualizationModels
```

Function gets VirtualizationModelId from GLPI from pipeline, and return Virtualization Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsVirtualizationModels
```

Function gets VirtualizationModelId from GLPI from pipeline (u can pass many ID's like that), and return Virtualization Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsVirtualizationModels -VirtualizationModelId 326
```

Function gets VirtualizationModelId from GLPI which is provided through -VirtualizationModelId after Function type, and return Virtualization Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsVirtualizationModels -VirtualizationModelId 326, 321
```

Function gets Virtualization Models Id from GLPI which is provided through -VirtualizationModelId keyword after Function type (u can provide many ID's like that), and return Virtualization Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsVirtualizationModels -VirtualizationModelName Fusion
```

Example will return glpi Virtualization Models, but what is the most important, Virtualization Models will be shown exactly as you see in glpi dropdown Virtualization Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Virtualization Models from GLPI

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

### -VirtualizationModelId
This parameter can take pipeline input, either, you can use this function with -VirtualizationModelId keyword.
Provide to this param VirtualizationModelId from GLPI Virtualization Models Bookmark

```yaml
Type: String[]
Parameter Sets: VirtualizationModelId
Aliases: VMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with VirtualizationModelId Parameter.
VirtualizationModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: VirtualizationModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -VirtualizationModelName
This parameter can take pipeline input, either, you can use this function with -VirtualizationModelId keyword.
Provide to this param Virtualization Models Name from GLPI Virtualization Models Bookmark

```yaml
Type: String
Parameter Sets: VirtualizationModelName
Aliases: VMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Virtualization Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Virtualization Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
