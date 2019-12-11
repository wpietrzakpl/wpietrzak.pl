---
title: Get-GlpiToolsDropdownsDeviceNetworkCardModels
---

## SYNOPSIS
Function is getting Device Network Card Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels [-All] [<CommonParameters>]
```

### DeviceNetworkCardModelId
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -DeviceNetworkCardModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceNetworkCardModelName
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -DeviceNetworkCardModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceNetworkCardModelId which you can find in GLPI website
Returns object with property's of Device Network Card Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -All
```

Example will return all Device Network Card Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceNetworkCardModels
```

Function gets DeviceNetworkCardModelId from GLPI from Pipline, and return Device Network Card Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceNetworkCardModels
```

Function gets DeviceNetworkCardModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Network Card Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -DeviceNetworkCardModelId 326
```

Function gets DeviceNetworkCardModelId from GLPI which is provided through -DeviceNetworkCardModelId after Function type, and return Device Network Card Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -DeviceNetworkCardModelId 326, 321
```

Function gets Device Network Card Models Id from GLPI which is provided through -DeviceNetworkCardModelId keyword after Function type (u can provide many ID's like that), and return Device Network Card Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceNetworkCardModels -DeviceNetworkCardModelName Fusion
```

Example will return glpi Device Network Card Models, but what is the most important, Device Network Card Models will be shown exactly as you see in glpi dropdown Device Network Card Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Network Card Models from GLPI

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

### -DeviceNetworkCardModelId
This parameter can take pipline input, either, you can use this function with -DeviceNetworkCardModelId keyword.
Provide to this param DeviceNetworkCardModelId from GLPI Device Network Card Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceNetworkCardModelId
Aliases: DNCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceNetworkCardModelId Parameter.
DeviceNetworkCardModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceNetworkCardModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceNetworkCardModelName
This parameter can take pipline input, either, you can use this function with -DeviceNetworkCardModelId keyword.
Provide to this param Device Network Card Models Name from GLPI Device Network Card Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceNetworkCardModelName
Aliases: DNCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Network Card Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Network Card Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
