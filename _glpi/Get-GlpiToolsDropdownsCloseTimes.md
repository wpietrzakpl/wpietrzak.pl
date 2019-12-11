---
title: Get-GlpiToolsDropdownsCloseTimes
---

## SYNOPSIS
Function is getting Close Times informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsCloseTimes [-All] [<CommonParameters>]
```

### CloseTimeId
```
Get-GlpiToolsDropdownsCloseTimes -CloseTimeId <String[]> [-Raw] [<CommonParameters>]
```

### CloseTimeName
```
Get-GlpiToolsDropdownsCloseTimes -CloseTimeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CloseTimeId which you can find in GLPI website
Returns object with property's of Close Times

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsCloseTimes -All
```

Example will return all Close Times from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsCloseTimes
```

Function gets CloseTimeId from GLPI from pipeline, and return Close Times object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsCloseTimes
```

Function gets CloseTimeId from GLPI from pipeline (u can pass many ID's like that), and return Close Times object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsCloseTimes -CloseTimeId 326
```

Function gets CloseTimeId from GLPI which is provided through -CloseTimeId after Function type, and return Close Times object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsCloseTimes -CloseTimeId 326, 321
```

Function gets Close Times Id from GLPI which is provided through -CloseTimeId keyword after Function type (u can provide many ID's like that), and return Close Times object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsCloseTimes -CloseTimeName Fusion
```

Example will return glpi Close Times, but what is the most important, Close Times will be shown exactly as you see in glpi dropdown Close Times.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Close Times from GLPI

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

### -CloseTimeId
This parameter can take pipeline input, either, you can use this function with -CloseTimeId keyword.
Provide to this param CloseTimeId from GLPI Close Times Bookmark

```yaml
Type: String[]
Parameter Sets: CloseTimeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CloseTimeId Parameter.
CloseTimeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CloseTimeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloseTimeName
This parameter can take pipeline input, either, you can use this function with -CloseTimeId keyword.
Provide to this param Close Times Name from GLPI Close Times Bookmark

```yaml
Type: String
Parameter Sets: CloseTimeName
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

### Close Times ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Close Times from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
