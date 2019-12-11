---
title: Get-GlpiToolsLines
---

## SYNOPSIS
Function is getting Line informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsLines [-All] [<CommonParameters>]
```

### LineId
```
Get-GlpiToolsLines -LineId <String[]> [-Raw] [<CommonParameters>]
```

### LineName
```
Get-GlpiToolsLines -LineName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on LineId which you can find in GLPI website
Returns object with property's of Line

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsLines -All
```

Example will return all Line from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsLines
```

Function gets LineId from GLPI from Pipline, and return Line object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsLines
```

Function gets LineId from GLPI from Pipline (u can pass many ID's like that), and return Line object

### EXAMPLE 4
```
Get-GlpiToolsLines -LineId 326
```

Function gets LineId from GLPI which is provided through -LineId after Function type, and return Line object

### EXAMPLE 5
```
Get-GlpiToolsLines -LineId 326, 321
```

Function gets Line Id from GLPI which is provided through -LineId keyword after Function type (u can provide many ID's like that), and return Line object

### EXAMPLE 6
```
Get-GlpiToolsLines -LineName Fusion
```

Example will return glpi Line, but what is the most important, Line will be shown exactly as you see in glpi dropdown Line.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Line from GLPI

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

### -LineId
This parameter can take pipline input, either, you can use this function with -LineId keyword.
Provide to this param LineId from GLPI Line Bookmark

```yaml
Type: String[]
Parameter Sets: LineId
Aliases: LID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with LineId Parameter.
LineId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: LineId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineName
This parameter can take pipline input, either, you can use this function with -LineId keyword.
Provide to this param Line Name from GLPI Line Bookmark

```yaml
Type: String
Parameter Sets: LineName
Aliases: LN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Line ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Line from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
