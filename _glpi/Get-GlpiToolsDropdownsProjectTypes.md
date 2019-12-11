---
title: Get-GlpiToolsDropdownsProjectTypes
---

## SYNOPSIS
Function is getting Project Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsProjectTypes [-All] [<CommonParameters>]
```

### ProjectTypeId
```
Get-GlpiToolsDropdownsProjectTypes -ProjectTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ProjectTypeName
```
Get-GlpiToolsDropdownsProjectTypes -ProjectTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProjectTypeId which you can find in GLPI website
Returns object with property's of Project Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsProjectTypes -All
```

Example will return all Project Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsProjectTypes
```

Function gets ProjectTypeId from GLPI from Pipline, and return Project Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsProjectTypes
```

Function gets ProjectTypeId from GLPI from Pipline (u can pass many ID's like that), and return Project Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsProjectTypes -ProjectTypeId 326
```

Function gets ProjectTypeId from GLPI which is provided through -ProjectTypeId after Function type, and return Project Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsProjectTypes -ProjectTypeId 326, 321
```

Function gets Project Types Id from GLPI which is provided through -ProjectTypeId keyword after Function type (u can provide many ID's like that), and return Project Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsProjectTypes -ProjectTypeName Fusion
```

Example will return glpi Project Types, but what is the most important, Project Types will be shown exactly as you see in glpi dropdown Project Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Project Types from GLPI

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

### -ProjectTypeId
This parameter can take pipline input, either, you can use this function with -ProjectTypeId keyword.
Provide to this param ProjectTypeId from GLPI Project Types Bookmark

```yaml
Type: String[]
Parameter Sets: ProjectTypeId
Aliases: PTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProjectTypeId Parameter.
ProjectTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProjectTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectTypeName
This parameter can take pipline input, either, you can use this function with -ProjectTypeId keyword.
Provide to this param Project Types Name from GLPI Project Types Bookmark

```yaml
Type: String
Parameter Sets: ProjectTypeName
Aliases: PTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Project Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Project Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
