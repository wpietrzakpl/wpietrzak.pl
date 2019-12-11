---
title: Get-GlpiToolsDropdownsDeviceGenericModels
---

## SYNOPSIS
Function is getting Device Generic Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceGenericModels [-All] [<CommonParameters>]
```

### DeviceGenericModelId
```
Get-GlpiToolsDropdownsDeviceGenericModels -DeviceGenericModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceGenericModelName
```
Get-GlpiToolsDropdownsDeviceGenericModels -DeviceGenericModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceGenericModelId which you can find in GLPI website
Returns object with property's of Device Generic Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceGenericModels -All
```

Example will return all Device Generic Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceGenericModels
```

Function gets DeviceGenericModelId from GLPI from Pipline, and return Device Generic Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceGenericModels
```

Function gets DeviceGenericModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Generic Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceGenericModels -DeviceGenericModelId 326
```

Function gets DeviceGenericModelId from GLPI which is provided through -DeviceGenericModelId after Function type, and return Device Generic Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceGenericModels -DeviceGenericModelId 326, 321
```

Function gets Device Generic Models Id from GLPI which is provided through -DeviceGenericModelId keyword after Function type (u can provide many ID's like that), and return Device Generic Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceGenericModels -DeviceGenericModelName Fusion
```

Example will return glpi Device Generic Models, but what is the most important, Device Generic Models will be shown exactly as you see in glpi dropdown Device Generic Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Generic Models from GLPI

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

### -DeviceGenericModelId
This parameter can take pipline input, either, you can use this function with -DeviceGenericModelId keyword.
Provide to this param DeviceGenericModelId from GLPI Device Generic Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceGenericModelId
Aliases: DGMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceGenericModelId Parameter.
DeviceGenericModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceGenericModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceGenericModelName
This parameter can take pipline input, either, you can use this function with -DeviceGenericModelId keyword.
Provide to this param Device Generic Models Name from GLPI Device Generic Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceGenericModelName
Aliases: DGMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Generic Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Generic Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
