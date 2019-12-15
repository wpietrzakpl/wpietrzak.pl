---
title: Get-GlpiToolsDropdownsComputerTypes
---

## SYNOPSIS
Function is getting ComputerType informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsComputerTypes [-All] [<CommonParameters>]
```

### ComputerTypeId
```
Get-GlpiToolsDropdownsComputerTypes -ComputerTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ComputerTypeName
```
Get-GlpiToolsDropdownsComputerTypes -ComputerTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ComputerTypeID which you can find in GLPI website
Returns object with property's of ComputerType

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsComputerTypes -All
```

Example will return all ComputerType from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsComputerTypes
```

Function gets ComputerTypeId from GLPI from Pipline, and return ComputerType object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsComputerTypes
```

Function gets ComputerTypeId from GLPI from Pipline (u can pass many ID's like that), and return ComputerType object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsComputerTypes -ComputerTypeId 326
```

Function gets ComputerTypeId from GLPI which is provided through -ComputerTypeId after Function type, and return ComputerType object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsComputerTypes -ComputerTypeId 326, 321
```

Function gets ComputerTypeId from GLPI which is provided through -ComputerTypeId keyword after Function type (u can provide many ID's like that), and return ComputerType object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsComputerTypes -ComputerType Fusion
```

Example will return glpi ComputerType, but what is the most important, ComputerType will be shown exactly as you see in glpi dropdown ComputerType.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all ComputerType from GLPI

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

### -ComputerTypeId
This parameter can take pipline input, either, you can use this function with -ComputerTypeId keyword.
Provide to this param ComputerType ID from GLPI ComputerType Bookmark

```yaml
Type: String[]
Parameter Sets: ComputerTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ComputerTypeId Parameter.
ComputerTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ComputerTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerTypeName

```yaml
Type: String
Parameter Sets: ComputerTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### ComputerType ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of ComputerType from GLPI
## NOTES
PSP 06/2019

## RELATED LINKS
