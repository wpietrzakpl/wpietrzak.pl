---
title: Get-GlpiToolsDropdownsOSServicePacks
---

## SYNOPSIS
Function is getting Operating Systems Service Packs informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSServicePacks [-All] [<CommonParameters>]
```

### OSServicePackId
```
Get-GlpiToolsDropdownsOSServicePacks -OSServicePackId <String[]> [-Raw] [<CommonParameters>]
```

### OSServicePackName
```
Get-GlpiToolsDropdownsOSServicePacks -OSServicePackName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSServicePackId which you can find in GLPI website
Returns object with property's of Operating Systems Service Packs

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSServicePacks -All
```

Example will return all Operating Systems Service Packs from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSServicePacks
```

Function gets OSServicePackId from GLPI from Pipline, and return Operating Systems Service Packs object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSServicePacks
```

Function gets OSServicePackId from GLPI from Pipline (u can pass many ID's like that), and return Operating Systems Service Packs object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSServicePacks -OSServicePackId 326
```

Function gets OSServicePackId from GLPI which is provided through -OSServicePackId after Function type, and return Operating Systems Service Packs object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSServicePacks -OSServicePackId 326, 321
```

Function gets Operating Systems Service PacksId from GLPI which is provided through -OSServicePackId keyword after Function type (u can provide many ID's like that), and return Operating Systems Service Packs object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSServicePacks -OSServicePackName Fusion
```

Example will return glpi Operating Systems Service Packs, but what is the most important, Operating Systems Service Packs will be shown exactly as you see in glpi dropdown Operating Systems Service Packs.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Operating Systems Service Packs from GLPI

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

### -OSServicePackId
This parameter can take pipline input, either, you can use this function with -OSServicePackId keyword.
Provide to this param OSServicePackId from GLPI Operating Systems Service Packs Bookmark

```yaml
Type: String[]
Parameter Sets: OSServicePackId
Aliases: OSSPID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSServicePackId Parameter.
OSServicePackId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSServicePackId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSServicePackName
This parameter can take pipline input, either, you can use this function with -OSServicePackId keyword.
Provide to this param Operating Systems Service Packs Name from GLPI Operating Systems Service Packs Bookmark

```yaml
Type: String
Parameter Sets: OSServicePackName
Aliases: OSPN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Operating Systems Service Packs ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Operating Systems Service Packs from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
