---
title: Get-GlpiToolsDropdownsLineOperators
---

## SYNOPSIS
Function is getting Line Operators informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsLineOperators [-All] [<CommonParameters>]
```

### LineOperatorId
```
Get-GlpiToolsDropdownsLineOperators -LineOperatorId <String[]> [-Raw] [<CommonParameters>]
```

### LineOperatorName
```
Get-GlpiToolsDropdownsLineOperators -LineOperatorName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on LineOperatorId which you can find in GLPI website
Returns object with property's of Line Operators

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsLineOperators -All
```

Example will return all Line Operators from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsLineOperators
```

Function gets LineOperatorId from GLPI from pipeline, and return Line Operators object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsLineOperators
```

Function gets LineOperatorId from GLPI from pipeline (u can pass many ID's like that), and return Line Operators object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsLineOperators -LineOperatorId 326
```

Function gets LineOperatorId from GLPI which is provided through -LineOperatorId after Function type, and return Line Operators object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsLineOperators -LineOperatorId 326, 321
```

Function gets Line Operators Id from GLPI which is provided through -LineOperatorId keyword after Function type (u can provide many ID's like that), and return Line Operators object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsLineOperators -LineOperatorName Fusion
```

Example will return glpi Line Operators, but what is the most important, Line Operators will be shown exactly as you see in glpi dropdown Line Operators.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Line Operators from GLPI

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

### -LineOperatorId
This parameter can take pipeline input, either, you can use this function with -LineOperatorId keyword.
Provide to this param LineOperatorId from GLPI Line Operators Bookmark

```yaml
Type: String[]
Parameter Sets: LineOperatorId
Aliases: LOID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with LineOperatorId Parameter.
LineOperatorId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: LineOperatorId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineOperatorName
This parameter can take pipeline input, either, you can use this function with -LineOperatorId keyword.
Provide to this param Line Operators Name from GLPI Line Operators Bookmark

```yaml
Type: String
Parameter Sets: LineOperatorName
Aliases: LON

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Line Operators ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Line Operators from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
