---
title: Get-GlpiToolsDropdownsSensorTypes
---

## SYNOPSIS
Function is getting Sensor Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsSensorTypes [-All] [<CommonParameters>]
```

### SensorTypeId
```
Get-GlpiToolsDropdownsSensorTypes -SensorTypeId <String[]> [-Raw] [<CommonParameters>]
```

### SensorTypeName
```
Get-GlpiToolsDropdownsSensorTypes -SensorTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SensorTypeId which you can find in GLPI website
Returns object with property's of Sensor Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsSensorTypes -All
```

Example will return all Sensor Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsSensorTypes
```

Function gets SensorTypeId from GLPI from Pipline, and return Sensor Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsSensorTypes
```

Function gets SensorTypeId from GLPI from Pipline (u can pass many ID's like that), and return Sensor Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsSensorTypes -SensorTypeId 326
```

Function gets SensorTypeId from GLPI which is provided through -SensorTypeId after Function type, and return Sensor Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsSensorTypes -SensorTypeId 326, 321
```

Function gets Sensor Types Id from GLPI which is provided through -SensorTypeId keyword after Function type (u can provide many ID's like that), and return Sensor Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsSensorTypes -SensorTypeName Fusion
```

Example will return glpi Sensor Types, but what is the most important, Sensor Types will be shown exactly as you see in glpi dropdown Sensor Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Sensor Types from GLPI

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

### -SensorTypeId
This parameter can take pipline input, either, you can use this function with -SensorTypeId keyword.
Provide to this param SensorTypeId from GLPI Sensor Types Bookmark

```yaml
Type: String[]
Parameter Sets: SensorTypeId
Aliases: STID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SensorTypeId Parameter.
SensorTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SensorTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SensorTypeName
This parameter can take pipline input, either, you can use this function with -SensorTypeId keyword.
Provide to this param Sensor Types Name from GLPI Sensor Types Bookmark

```yaml
Type: String
Parameter Sets: SensorTypeName
Aliases: STN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Sensor Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Sensor Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
