---
title: Get-GlpiToolsProjects
---

## SYNOPSIS
Function is getting Projects informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsProjects [-All] [<CommonParameters>]
```

### ProjectId
```
Get-GlpiToolsProjects -ProjectId <String[]> [-Raw] [<CommonParameters>]
```

### ProjectName
```
Get-GlpiToolsProjects -ProjectName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProjectId which you can find in GLPI website
Returns object with property's of Projects

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsProjects -All
```

Example will return all Projects from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsProjects
```

Function gets ProjectId from GLPI from Pipline, and return Projects object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsProjects
```

Function gets ProjectId from GLPI from Pipline (u can pass many ID's like that), and return Projects object

### EXAMPLE 4
```
Get-GlpiToolsProjects -ProjectId 326
```

Function gets ProjectId from GLPI which is provided through -ProjectId after Function type, and return Projects object

### EXAMPLE 5
```
Get-GlpiToolsProjects -ProjectId 326, 321
```

Function gets Projects Id from GLPI which is provided through -ProjectId keyword after Function type (u can provide many ID's like that), and return Projects object

### EXAMPLE 6
```
Get-GlpiToolsProjects -ProjectName Fusion
```

Example will return glpi Projects, but what is the most important, Projects will be shown exactly as you see in glpi dropdown Projects.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Projects from GLPI

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

### -ProjectId
This parameter can take pipline input, either, you can use this function with -ProjectId keyword.
Provide to this param ProjectId from GLPI Projects Bookmark

```yaml
Type: String[]
Parameter Sets: ProjectId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProjectId Parameter.
ProjectId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProjectId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProjectName
This parameter can take pipline input, either, you can use this function with -ProjectId keyword.
Provide to this param Projects Name from GLPI Projects Bookmark

```yaml
Type: String
Parameter Sets: ProjectName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Projects ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Projects from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
