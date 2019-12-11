---
title: Get-GlpiToolsDropdownsProjectTasksTypes
---

## SYNOPSIS
Function is getting Project Tasks Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsProjectTasksTypes [-All] [<CommonParameters>]
```

### ProjectTaskTypeId
```
Get-GlpiToolsDropdownsProjectTasksTypes -ProjectTaskTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ProjectTaskTypeName
```
Get-GlpiToolsDropdownsProjectTasksTypes -ProjectTaskTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProjectTaskTypeId which you can find in GLPI website
Returns object with property's of Project Tasks Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsProjectTasksTypes -All
```

Example will return all Project Tasks Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsProjectTasksTypes
```

Function gets ProjectTaskTypeId from GLPI from Pipline, and return Project Tasks Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsProjectTasksTypes
```

Function gets ProjectTaskTypeId from GLPI from Pipline (u can pass many ID's like that), and return Project Tasks Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsProjectTasksTypes -ProjectTaskTypeId 326
```

Function gets ProjectTaskTypeId from GLPI which is provided through -ProjectTaskTypeId after Function type, and return Project Tasks Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsProjectTasksTypes -ProjectTaskTypeId 326, 321
```

Function gets Project Tasks Types Id from GLPI which is provided through -ProjectTaskTypeId keyword after Function type (u can provide many ID's like that), and return Project Tasks Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsProjectTasksTypes -ProjectTaskTypeName Fusion
```

Example will return glpi Project Tasks Types, but what is the most important, Project Tasks Types will be shown exactly as you see in glpi dropdown Project Tasks Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Project Tasks Types from GLPI

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

### -ProjectTaskTypeId
This parameter can take pipline input, either, you can use this function with -ProjectTaskTypeId keyword.
Provide to this param ProjectTaskTypeId from GLPI Project Tasks Types Bookmark

```yaml
Type: String[]
Parameter Sets: ProjectTaskTypeId
Aliases: PTTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProjectTaskTypeId Parameter.
ProjectTaskTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProjectTaskTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectTaskTypeName
This parameter can take pipline input, either, you can use this function with -ProjectTaskTypeId keyword.
Provide to this param Project Tasks Types Name from GLPI Project Tasks Types Bookmark

```yaml
Type: String
Parameter Sets: ProjectTaskTypeName
Aliases: PTTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Project Tasks Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Project Tasks Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
