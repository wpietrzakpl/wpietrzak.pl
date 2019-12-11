---
title: Get-GlpiToolsDropdownsRequestSources
---

## SYNOPSIS
Function is getting Request Sources informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsRequestSources [-All] [<CommonParameters>]
```

### RequestSourceId
```
Get-GlpiToolsDropdownsRequestSources -RequestSourceId <String[]> [-Raw] [<CommonParameters>]
```

### RequestSourceName
```
Get-GlpiToolsDropdownsRequestSources -RequestSourceName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on RequestSourceId which you can find in GLPI website
Returns object with property's of Request Sources

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsRequestSources -All
```

Example will return all Request Sources from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsRequestSources
```

Function gets RequestSourceId from GLPI from Pipline, and return Request Sources object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsRequestSources
```

Function gets RequestSourceId from GLPI from Pipline (u can pass many ID's like that), and return Request Sources object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsRequestSources -RequestSourceId 326
```

Function gets RequestSourceId from GLPI which is provided through -RequestSourceId after Function type, and return Request Sources object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsRequestSources -RequestSourceId 326, 321
```

Function gets Request Sources Id from GLPI which is provided through -RequestSourceId keyword after Function type (u can provide many ID's like that), and return Request Sources object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsRequestSources -RequestSourceName Fusion
```

Example will return glpi Request Sources, but what is the most important, Request Sources will be shown exactly as you see in glpi dropdown Request Sources.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Request Sources from GLPI

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

### -RequestSourceId
This parameter can take pipline input, either, you can use this function with -RequestSourceId keyword.
Provide to this param RequestSourceId from GLPI Request Sources Bookmark

```yaml
Type: String[]
Parameter Sets: RequestSourceId
Aliases: RSID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RequestSourceId Parameter.
RequestSourceId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RequestSourceId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestSourceName
This parameter can take pipline input, either, you can use this function with -RequestSourceId keyword.
Provide to this param Request Sources Name from GLPI Request Sources Bookmark

```yaml
Type: String
Parameter Sets: RequestSourceName
Aliases: RSN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Request Sources ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Request Sources from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
