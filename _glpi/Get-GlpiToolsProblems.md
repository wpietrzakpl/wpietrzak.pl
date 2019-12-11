---
title: Get-GlpiToolsProblems
---

## SYNOPSIS
Function is getting Problem informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsProblems [-All] [<CommonParameters>]
```

### ProblemId
```
Get-GlpiToolsProblems -ProblemId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### ProblemName
```
Get-GlpiToolsProblems -ProblemName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProblemID which you can find in GLPI website
Returns object with property's of Problem

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsProblems
```

Function gets ProblemID from GLPI from Pipline, and return Problem object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsProblems
```

Function gets ProblemID from GLPI from Pipline (u can pass many ID's like that), and return Problem object

### EXAMPLE 3
```
Get-GlpiToolsProblems -ProblemId 326
```

Function gets ProblemID from GLPI which is provided through -ProblemId after Function type, and return Problem object

### EXAMPLE 4
```
Get-GlpiToolsProblems -ProblemId 326, 321
```

Function gets ProblemID from GLPI which is provided through -ProblemId keyword after Function type (u can provide many ID's like that), and return Problem object

### EXAMPLE 5
```
Get-GlpiToolsProblems -ProblemId 234 -Raw
```

Example will show Problem with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsProblems -Raw
```

Example will show Problem with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsProblems -ProblemName glpi
```

Example will return glpi Problem, but what is the most important, Problem will be shown exacly as you see in glpi Problems tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsProblems -ProblemName glpi -SearchInTrash Yes
```

Example will return glpi Problem, but from trash

## PARAMETERS

### -All
This parameter will return all Problems from GLPI

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

### -ProblemId
This parameter can take pipline input, either, you can use this function with -ProblemId keyword.
Provide to this param Problem ID from GLPI Problems Bookmark

```yaml
Type: String[]
Parameter Sets: ProblemId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProblemId Parameter.
ProblemId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProblemId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProblemName
Provide to this param Problem Name from GLPI Problems Bookmark

```yaml
Type: String
Parameter Sets: ProblemName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with ProblemName Parameter.
If you want Search for Problem name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: ProblemName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with ProblemId Parameter. 
If you want to get additional parameter of Problem object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: ProblemId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Problem ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Problems from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
