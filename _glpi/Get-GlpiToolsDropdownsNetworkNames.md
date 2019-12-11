---
title: Get-GlpiToolsDropdownsNetworkNames
---

## SYNOPSIS
Function is getting Network Names informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsNetworkNames [-All] [<CommonParameters>]
```

### NetworkNameId
```
Get-GlpiToolsDropdownsNetworkNames -NetworkNameId <String[]> [-Raw] [<CommonParameters>]
```

### NetworkNameName
```
Get-GlpiToolsDropdownsNetworkNames -NetworkNameName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkNameId which you can find in GLPI website
Returns object with property's of Network Names

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsNetworkNames -All
```

Example will return all Network Names from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsNetworkNames
```

Function gets NetworkNameId from GLPI from pipeline, and return Network Names object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsNetworkNames
```

Function gets NetworkNameId from GLPI from pipeline (u can pass many ID's like that), and return Network Names object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsNetworkNames -NetworkNameId 326
```

Function gets NetworkNameId from GLPI which is provided through -NetworkNameId after Function type, and return Network Names object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsNetworkNames -NetworkNameId 326, 321
```

Function gets Network Names Id from GLPI which is provided through -NetworkNameId keyword after Function type (u can provide many ID's like that), and return Network Names object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsNetworkNames -NetworkNameName Fusion
```

Example will return glpi Network Names, but what is the most important, Network Names will be shown exactly as you see in glpi dropdown Network Names.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Network Names from GLPI

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

### -NetworkNameId
This parameter can take pipeline input, either, you can use this function with -NetworkNameId keyword.
Provide to this param NetworkNameId from GLPI Network Names Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkNameId
Aliases: NNID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkNameId Parameter.
NetworkNameId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkNameId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkNameName
This parameter can take pipeline input, either, you can use this function with -NetworkNameId keyword.
Provide to this param Network Names Name from GLPI Network Names Bookmark

```yaml
Type: String
Parameter Sets: NetworkNameName
Aliases: NNN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Network Names ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Network Names from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
