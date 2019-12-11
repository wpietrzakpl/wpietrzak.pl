---
title: Get-GlpiToolsDropdownsMonitorTypes
---

## SYNOPSIS
Function is getting Monitor Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsMonitorTypes [-All] [<CommonParameters>]
```

### MonitorTypeId
```
Get-GlpiToolsDropdownsMonitorTypes -MonitorTypeId <String[]> [-Raw] [<CommonParameters>]
```

### MonitorTypeName
```
Get-GlpiToolsDropdownsMonitorTypes -MonitorTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on MonitorTypeId which you can find in GLPI website
Returns object with property's of Monitor Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsMonitorTypes -All
```

Example will return all Monitor Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsMonitorTypes
```

Function gets MonitorTypeId from GLPI from Pipline, and return Monitor Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsMonitorTypes
```

Function gets MonitorTypeId from GLPI from Pipline (u can pass many ID's like that), and return Monitor Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsMonitorTypes -MonitorTypeId 326
```

Function gets MonitorTypeId from GLPI which is provided through -MonitorTypeId after Function type, and return Monitor Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsMonitorTypes -MonitorTypeId 326, 321
```

Function gets Monitor Types Id from GLPI which is provided through -MonitorTypeId keyword after Function type (u can provide many ID's like that), and return Monitor Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsMonitorTypes -MonitorTypeName Fusion
```

Example will return glpi Monitor Types, but what is the most important, Monitor Types will be shown exactly as you see in glpi dropdown Monitor Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Monitor Types from GLPI

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

### -MonitorTypeId
This parameter can take pipline input, either, you can use this function with -MonitorTypeId keyword.
Provide to this param MonitorTypeId from GLPI Monitor Types Bookmark

```yaml
Type: String[]
Parameter Sets: MonitorTypeId
Aliases: MTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with MonitorTypeId Parameter.
MonitorTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: MonitorTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MonitorTypeName
This parameter can take pipline input, either, you can use this function with -MonitorTypeId keyword.
Provide to this param Monitor Types Name from GLPI Monitor Types Bookmark

```yaml
Type: String
Parameter Sets: MonitorTypeName
Aliases: MTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Monitor Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Monitor Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
