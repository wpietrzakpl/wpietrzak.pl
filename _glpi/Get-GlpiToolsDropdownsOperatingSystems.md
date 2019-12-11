---
title: Get-GlpiToolsDropdownsOperatingSystems
---

## SYNOPSIS
Function is getting Operating Systems informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOperatingSystems [-All] [<CommonParameters>]
```

### OperatingSystemId
```
Get-GlpiToolsDropdownsOperatingSystems -OperatingSystemId <String[]> [-Raw] [<CommonParameters>]
```

### OperatingSystemName
```
Get-GlpiToolsDropdownsOperatingSystems -OperatingSystemName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OperatingSystemId which you can find in GLPI website
Returns object with property's of Operating Systems

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOperatingSystems -All
```

Example will return all Operating Systems from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOperatingSystems
```

Function gets OperatingSystemId from GLPI from Pipline, and return Operating Systems object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOperatingSystems
```

Function gets OperatingSystemId from GLPI from Pipline (u can pass many ID's like that), and return Operating Systems object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOperatingSystems -OperatingSystemId 326
```

Function gets OperatingSystemId from GLPI which is provided through -OperatingSystemId after Function type, and return Operating Systems object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOperatingSystems -OperatingSystemId 326, 321
```

Function gets Operating SystemsId from GLPI which is provided through -OperatingSystemId keyword after Function type (u can provide many ID's like that), and return Operating Systems object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOperatingSystems -OperatingSystemName Fusion
```

Example will return glpi Operating Systems, but what is the most important, Operating Systems will be shown exactly as you see in glpi dropdown Operating Systems.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Operating Systems from GLPI

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

### -OperatingSystemId
This parameter can take pipline input, either, you can use this function with -OperatingSystemId keyword.
Provide to this param OperatingSystemId from GLPI Operating Systems Bookmark

```yaml
Type: String[]
Parameter Sets: OperatingSystemId
Aliases: OSID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OperatingSystemId Parameter.
OperatingSystemId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OperatingSystemId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OperatingSystemName
This parameter can take pipline input, either, you can use this function with -OperatingSystemId keyword.
Provide to this param Operating Systems Name from GLPI Operating Systems Bookmark

```yaml
Type: String
Parameter Sets: OperatingSystemName
Aliases: OSN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Operating Systems ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Operating Systems from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
