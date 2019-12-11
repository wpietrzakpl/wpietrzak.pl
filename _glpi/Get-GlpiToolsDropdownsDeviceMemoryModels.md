---
title: Get-GlpiToolsDropdownsDeviceMemoryModels
---

## SYNOPSIS
Function is getting Device Memory Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceMemoryModels [-All] [<CommonParameters>]
```

### DeviceMemoryModelId
```
Get-GlpiToolsDropdownsDeviceMemoryModels -DeviceMemoryModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceMemoryModelName
```
Get-GlpiToolsDropdownsDeviceMemoryModels -DeviceMemoryModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceMemoryModelId which you can find in GLPI website
Returns object with property's of Device Memory Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceMemoryModels -All
```

Example will return all Device Memory Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceMemoryModels
```

Function gets DeviceMemoryModelId from GLPI from Pipline, and return Device Memory Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceMemoryModels
```

Function gets DeviceMemoryModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Memory Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceMemoryModels -DeviceMemoryModelId 326
```

Function gets DeviceMemoryModelId from GLPI which is provided through -DeviceMemoryModelId after Function type, and return Device Memory Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceMemoryModels -DeviceMemoryModelId 326, 321
```

Function gets Device Memory Models Id from GLPI which is provided through -DeviceMemoryModelId keyword after Function type (u can provide many ID's like that), and return Device Memory Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceMemoryModels -DeviceMemoryModelName Fusion
```

Example will return glpi Device Memory Models, but what is the most important, Device Memory Models will be shown exactly as you see in glpi dropdown Device Memory Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Memory Models from GLPI

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

### -DeviceMemoryModelId
This parameter can take pipline input, either, you can use this function with -DeviceMemoryModelId keyword.
Provide to this param DeviceMemoryModelId from GLPI Device Memory Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceMemoryModelId
Aliases: DMMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceMemoryModelId Parameter.
DeviceMemoryModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceMemoryModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceMemoryModelName
This parameter can take pipline input, either, you can use this function with -DeviceMemoryModelId keyword.
Provide to this param Device Memory Models Name from GLPI Device Memory Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceMemoryModelName
Aliases: DMMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Memory Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Memory Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
