---
title: Get-GlpiToolsDropdownsDeviceCaseModels
---

## SYNOPSIS
Function is getting Device Case Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceCaseModels [-All] [<CommonParameters>]
```

### DeviceCaseModelId
```
Get-GlpiToolsDropdownsDeviceCaseModels -DeviceCaseModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceCaseModelName
```
Get-GlpiToolsDropdownsDeviceCaseModels -DeviceCaseModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceCaseModelId which you can find in GLPI website
Returns object with property's of Device Case Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceCaseModels -All
```

Example will return all Device Case Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceCaseModels
```

Function gets DeviceCaseModelId from GLPI from Pipline, and return Device Case Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceCaseModels
```

Function gets DeviceCaseModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Case Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceCaseModels -DeviceCaseModelId 326
```

Function gets DeviceCaseModelId from GLPI which is provided through -DeviceCaseModelId after Function type, and return Device Case Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceCaseModels -DeviceCaseModelId 326, 321
```

Function gets Device Case Models Id from GLPI which is provided through -DeviceCaseModelId keyword after Function type (u can provide many ID's like that), and return Device Case Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceCaseModels -DeviceCaseModelName Fusion
```

Example will return glpi Device Case Models, but what is the most important, Device Case Models will be shown exactly as you see in glpi dropdown Device Case Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Case Models from GLPI

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

### -DeviceCaseModelId
This parameter can take pipline input, either, you can use this function with -DeviceCaseModelId keyword.
Provide to this param DeviceCaseModelId from GLPI Device Case Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceCaseModelId
Aliases: DCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceCaseModelId Parameter.
DeviceCaseModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceCaseModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceCaseModelName
This parameter can take pipline input, either, you can use this function with -DeviceCaseModelId keyword.
Provide to this param Device Case Models Name from GLPI Device Case Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceCaseModelName
Aliases: DCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Case Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Case Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
