---
title: Get-GlpiToolsDropdownsMonitorModels
---

## SYNOPSIS
Function is getting MonitorModel informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsMonitorModels [-All] [<CommonParameters>]
```

### MonitorModelId
```
Get-GlpiToolsDropdownsMonitorModels -MonitorModelId <String[]> [-Raw] [<CommonParameters>]
```

### MonitorModelName
```
Get-GlpiToolsDropdownsMonitorModels -MonitorModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on MonitorModelId which you can find in GLPI website
Returns object with property's of MonitorModel

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsMonitorModels -All
```

Example will return all MonitorModel from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsMonitorModels
```

Function gets MonitorModelId from GLPI from Pipline, and return MonitorModel object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsMonitorModels
```

Function gets MonitorModelId from GLPI from Pipline (u can pass many ID's like that), and return MonitorModel object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsMonitorModels -MonitorModelId 326
```

Function gets MonitorModelId from GLPI which is provided through -MonitorModelId after Function type, and return MonitorModel object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsMonitorModels -MonitorModelId 326, 321
```

Function gets MonitorModelId from GLPI which is provided through -MonitorModelId keyword after Function type (u can provide many ID's like that), and return MonitorModel object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsMonitorModels -MonitorModelName Fusion
```

Example will return glpi MonitorModel, but what is the most important, MonitorModel will be shown exactly as you see in glpi dropdown MonitorModel.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all MonitorModel from GLPI

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

### -MonitorModelId
This parameter can take pipline input, either, you can use this function with -MonitorModelId keyword.
Provide to this param MonitorModel ID from GLPI MonitorModel Bookmark

```yaml
Type: String[]
Parameter Sets: MonitorModelId
Aliases: MMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with MonitorModelId Parameter.
MonitorModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: MonitorModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MonitorModelName
Example will return glpi Monitor Model, but what is the most important, Monitor model will be shown exacly as you see in glpi Monitor models tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

```yaml
Type: String
Parameter Sets: MonitorModelName
Aliases: MMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### MonitorModel ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of MonitorModel from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
