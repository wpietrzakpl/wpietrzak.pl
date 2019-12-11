---
title: Get-GlpiToolsDropdownsOSVersions
---

## SYNOPSIS
Function is getting Operating Systems Versions informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSVersions [-All] [<CommonParameters>]
```

### OSVersionId
```
Get-GlpiToolsDropdownsOSVersions -OSVersionId <String[]> [-Raw] [<CommonParameters>]
```

### OSVersionName
```
Get-GlpiToolsDropdownsOSVersions -OSVersionName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSVersionId which you can find in GLPI website
Returns object with property's of Operating Systems Versions

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSVersions -All
```

Example will return all Operating Systems Versions from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSVersions
```

Function gets OSVersionId from GLPI from Pipline, and return Operating Systems Versions object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSVersions
```

Function gets OSVersionId from GLPI from Pipline (u can pass many ID's like that), and return Operating Systems Versions object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSVersions -OSVersionId 326
```

Function gets OSVersionId from GLPI which is provided through -OSVersionId after Function type, and return Operating Systems Versions object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSVersions -OSVersionId 326, 321
```

Function gets Operating Systems VersionsId from GLPI which is provided through -OSVersionId keyword after Function type (u can provide many ID's like that), and return Operating Systems Versions object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSVersions -OSVersionName Fusion
```

Example will return glpi Operating Systems Versions, but what is the most important, Operating Systems Versions will be shown exactly as you see in glpi dropdown Operating Systems Versions.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Operating Systems Versions from GLPI

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

### -OSVersionId
This parameter can take pipline input, either, you can use this function with -OSVersionId keyword.
Provide to this param OSVersionId from GLPI Operating Systems Versions Bookmark

```yaml
Type: String[]
Parameter Sets: OSVersionId
Aliases: OSVID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSVersionId Parameter.
OSVersionId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSVersionId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSVersionName
This parameter can take pipline input, either, you can use this function with -OSVersionId keyword.
Provide to this param Operating Systems Versions Name from GLPI Operating Systems Versions Bookmark

```yaml
Type: String
Parameter Sets: OSVersionName
Aliases: OSVN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Operating Systems Versions ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Operating Systems Versions from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
