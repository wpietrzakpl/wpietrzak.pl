---
title: Get-GlpiToolsDropdownsLineTypes
---

## SYNOPSIS
Function is getting Line Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsLineTypes [-All] [<CommonParameters>]
```

### LineTypeId
```
Get-GlpiToolsDropdownsLineTypes -LineTypeId <String[]> [-Raw] [<CommonParameters>]
```

### LineTypeName
```
Get-GlpiToolsDropdownsLineTypes -LineTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on LineTypeId which you can find in GLPI website
Returns object with property's of Line Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsLineTypes -All
```

Example will return all Line Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsLineTypes
```

Function gets LineTypeId from GLPI from Pipline, and return Line Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsLineTypes
```

Function gets LineTypeId from GLPI from Pipline (u can pass many ID's like that), and return Line Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsLineTypes -LineTypeId 326
```

Function gets LineTypeId from GLPI which is provided through -LineTypeId after Function type, and return Line Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsLineTypes -LineTypeId 326, 321
```

Function gets Line Types Id from GLPI which is provided through -LineTypeId keyword after Function type (u can provide many ID's like that), and return Line Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsLineTypes -LineTypeName Fusion
```

Example will return glpi Line Types, but what is the most important, Line Types will be shown exactly as you see in glpi dropdown Line Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Line Types from GLPI

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

### -LineTypeId
This parameter can take pipline input, either, you can use this function with -LineTypeId keyword.
Provide to this param LineTypeId from GLPI Line Types Bookmark

```yaml
Type: String[]
Parameter Sets: LineTypeId
Aliases: LTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with LineTypeId Parameter.
LineTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: LineTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineTypeName
This parameter can take pipline input, either, you can use this function with -LineTypeId keyword.
Provide to this param Line Types Name from GLPI Line Types Bookmark

```yaml
Type: String
Parameter Sets: LineTypeName
Aliases: LTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Line Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Line Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
