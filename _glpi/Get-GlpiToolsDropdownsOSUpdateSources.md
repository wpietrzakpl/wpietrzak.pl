---
title: Get-GlpiToolsDropdownsOSUpdateSources
---

## SYNOPSIS
Function is getting Update Sources informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSUpdateSources [-All] [<CommonParameters>]
```

### UpdateSourcesId
```
Get-GlpiToolsDropdownsOSUpdateSources -UpdateSourcesId <String[]> [<CommonParameters>]
```

### UpdateSourcesName
```
Get-GlpiToolsDropdownsOSUpdateSources -UpdateSourcesName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on UpdateSourcesID which you can find in GLPI website
Returns object with property's of Update Sources

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSUpdateSources -All
```

Example will return all Update Sources from Update Sources.

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSUpdateSources
```

Function gets UpdateSourcesID from GLPI from Pipline, and return Update Sources object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSUpdateSources
```

Function gets UpdateSourcesID from GLPI from Pipline (u can pass many ID's like that), and return Update Sources object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSUpdateSources -UpdateSourcesId 326
```

Function gets UpdateSourcesID from GLPI which is provided through -UpdateSourcesId after Function type, and return Update Sources object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSUpdateSources -UpdateSourcesId 326, 321
```

Function gets UpdateSourcesID from GLPI which is provided through -UpdateSourcesId keyword after Function type (u can provide many ID's like that), and return Update Sources object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSUpdateSources -UpdateSourcesName glpi
```

Example will return glpi Update Sources, but what is the most important, Update Sources will be shown exactly as you see in glpi Update Sources tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Update Sources from GLPI

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

### -UpdateSourcesId
This parameter can take pipline input, either, you can use this function with -UpdateSourcesId keyword.
Provide to this param Update Sources ID from GLPI Update Sources Bookmark

```yaml
Type: String[]
Parameter Sets: UpdateSourcesId
Aliases: USID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -UpdateSourcesName
Provide to this param Update Sources Name from GLPI Update Sources Bookmark

```yaml
Type: String
Parameter Sets: UpdateSourcesName
Aliases: USN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Update Sources ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Update Sources from GLPI
## NOTES
PSP 03/2019

## RELATED LINKS
