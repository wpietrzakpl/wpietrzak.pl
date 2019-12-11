---
title: Get-GlpiToolsDropdownsDeviceSoundCardModels
---

## SYNOPSIS
Function is getting Device Sound Card Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDeviceSoundCardModels [-All] [<CommonParameters>]
```

### DeviceSoundCardModelId
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -DeviceSoundCardModelId <String[]> [-Raw] [<CommonParameters>]
```

### DeviceSoundCardModelName
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -DeviceSoundCardModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DeviceSoundCardModelId which you can find in GLPI website
Returns object with property's of Device Sound Card Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -All
```

Example will return all Device Sound Card Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDeviceSoundCardModels
```

Function gets DeviceSoundCardModelId from GLPI from Pipline, and return Device Sound Card Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDeviceSoundCardModels
```

Function gets DeviceSoundCardModelId from GLPI from Pipline (u can pass many ID's like that), and return Device Sound Card Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -DeviceSoundCardModelId 326
```

Function gets DeviceSoundCardModelId from GLPI which is provided through -DeviceSoundCardModelId after Function type, and return Device Sound Card Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -DeviceSoundCardModelId 326, 321
```

Function gets Device Sound Card Models Id from GLPI which is provided through -DeviceSoundCardModelId keyword after Function type (u can provide many ID's like that), and return Device Sound Card Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDeviceSoundCardModels -DeviceSoundCardModelName Fusion
```

Example will return glpi Device Sound Card Models, but what is the most important, Device Sound Card Models will be shown exactly as you see in glpi dropdown Device Sound Card Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Device Sound Card Models from GLPI

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

### -DeviceSoundCardModelId
This parameter can take pipline input, either, you can use this function with -DeviceSoundCardModelId keyword.
Provide to this param DeviceSoundCardModelId from GLPI Device Sound Card Models Bookmark

```yaml
Type: String[]
Parameter Sets: DeviceSoundCardModelId
Aliases: DSCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DeviceSoundCardModelId Parameter.
DeviceSoundCardModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DeviceSoundCardModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceSoundCardModelName
This parameter can take pipline input, either, you can use this function with -DeviceSoundCardModelId keyword.
Provide to this param Device Sound Card Models Name from GLPI Device Sound Card Models Bookmark

```yaml
Type: String
Parameter Sets: DeviceSoundCardModelName
Aliases: DSCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Device Sound Card Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Device Sound Card Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
