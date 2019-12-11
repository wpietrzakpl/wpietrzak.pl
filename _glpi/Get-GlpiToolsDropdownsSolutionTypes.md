---
title: Get-GlpiToolsDropdownsSolutionTypes
---

## SYNOPSIS
Function is getting Solution Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsSolutionTypes [-All] [<CommonParameters>]
```

### SolutionTypesId
```
Get-GlpiToolsDropdownsSolutionTypes -SolutionTypesId <String[]> [-Raw] [<CommonParameters>]
```

### SolutionTypesName
```
Get-GlpiToolsDropdownsSolutionTypes -SolutionTypesName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SolutionTypesId which you can find in GLPI website
Returns object with property's of Solution Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsSolutionTypes -All
```

Example will return all Solution Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsSolutionTypes
```

Function gets SolutionTypesId from GLPI from Pipline, and return Solution Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsSolutionTypes
```

Function gets SolutionTypesId from GLPI from Pipline (u can pass many ID's like that), and return Solution Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsSolutionTypes -SolutionTypesId 326
```

Function gets SolutionTypesId from GLPI which is provided through -SolutionTypesId after Function type, and return Solution Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsSolutionTypes -SolutionTypesId 326, 321
```

Function gets Solution Types Id from GLPI which is provided through -SolutionTypesId keyword after Function type (u can provide many ID's like that), and return Solution Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsSolutionTypes -SolutionTypesName Fusion
```

Example will return glpi Solution Types, but what is the most important, Solution Types will be shown exactly as you see in glpi dropdown Solution Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Solution Types from GLPI

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

### -SolutionTypesId
This parameter can take pipline input, either, you can use this function with -SolutionTypesId keyword.
Provide to this param SolutionTypesId from GLPI Solution Types Bookmark

```yaml
Type: String[]
Parameter Sets: SolutionTypesId
Aliases: STID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SolutionTypesId Parameter.
SolutionTypesId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SolutionTypesId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SolutionTypesName
This parameter can take pipline input, either, you can use this function with -SolutionTypesId keyword.
Provide to this param Solution Types Name from GLPI Solution Types Bookmark

```yaml
Type: String
Parameter Sets: SolutionTypesName
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

### Solution Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Solution Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
