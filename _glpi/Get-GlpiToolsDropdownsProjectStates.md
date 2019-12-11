---
title: Get-GlpiToolsDropdownsProjectStates
---

## SYNOPSIS
Function is getting Project States informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsProjectStates [-All] [<CommonParameters>]
```

### ProjectStateId
```
Get-GlpiToolsDropdownsProjectStates -ProjectStateId <String[]> [-Raw] [<CommonParameters>]
```

### ProjectStateName
```
Get-GlpiToolsDropdownsProjectStates -ProjectStateName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProjectStateId which you can find in GLPI website
Returns object with property's of Project States

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsProjectStates -All
```

Example will return all Project States from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsProjectStates
```

Function gets ProjectStateId from GLPI from Pipline, and return Project States object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsProjectStates
```

Function gets ProjectStateId from GLPI from Pipline (u can pass many ID's like that), and return Project States object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsProjectStates -ProjectStateId 326
```

Function gets ProjectStateId from GLPI which is provided through -ProjectStateId after Function type, and return Project States object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsProjectStates -ProjectStateId 326, 321
```

Function gets Project States Id from GLPI which is provided through -ProjectStateId keyword after Function type (u can provide many ID's like that), and return Project States object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsProjectStates -ProjectStateName Fusion
```

Example will return glpi Project States, but what is the most important, Project States will be shown exactly as you see in glpi dropdown Project States.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Project States from GLPI

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

### -ProjectStateId
This parameter can take pipline input, either, you can use this function with -ProjectStateId keyword.
Provide to this param ProjectStateId from GLPI Project States Bookmark

```yaml
Type: String[]
Parameter Sets: ProjectStateId
Aliases: PSID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProjectStateId Parameter.
ProjectStateId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProjectStateId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectStateName
This parameter can take pipline input, either, you can use this function with -ProjectStateId keyword.
Provide to this param Project States Name from GLPI Project States Bookmark

```yaml
Type: String
Parameter Sets: ProjectStateName
Aliases: PSN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Project States ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Project States from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
