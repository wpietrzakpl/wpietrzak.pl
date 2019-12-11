---
title: Get-GlpiToolsDropdownsBlacklists
---

## SYNOPSIS
Function is getting Blacklists informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsBlacklists [-All] [<CommonParameters>]
```

### BlacklistsId
```
Get-GlpiToolsDropdownsBlacklists -BlacklistsId <String[]> [-Raw] [<CommonParameters>]
```

### BlacklistsName
```
Get-GlpiToolsDropdownsBlacklists -BlacklistsName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on BlacklistsId which you can find in GLPI website
Returns object with property's of Blacklists

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsBlacklists -All
```

Example will return all Blacklists from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsBlacklists
```

Function gets BlacklistsId from GLPI from Pipline, and return Blacklists object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsBlacklists
```

Function gets BlacklistsId from GLPI from Pipline (u can pass many ID's like that), and return Blacklists object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsBlacklists -BlacklistsId 326
```

Function gets BlacklistsId from GLPI which is provided through -BlacklistsId after Function type, and return Blacklists object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsBlacklists -BlacklistsId 326, 321
```

Function gets BlacklistsId from GLPI which is provided through -BlacklistsId keyword after Function type (u can provide many ID's like that), and return Blacklists object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsBlacklists -BlacklistsId Fusion
```

Example will return glpi Blacklists, but what is the most important, Blacklists will be shown exactly as you see in glpi dropdown Blacklists.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Blacklists from GLPI

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

### -BlacklistsId
This parameter can take pipline input, either, you can use this function with -BlacklistsId keyword.
Provide to this param Blacklists ID from GLPI Blacklists Bookmark

```yaml
Type: String[]
Parameter Sets: BlacklistsId
Aliases: BID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with BlacklistsId Parameter.
BlacklistsId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: BlacklistsId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BlacklistsName
This parameter can take pipline input, either, you can use this function with -BlacklistsId keyword.
Provide to this param Blacklists Name from GLPI Blacklists Bookmark

```yaml
Type: String
Parameter Sets: BlacklistsName
Aliases: BN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Blacklists ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Blacklists from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
