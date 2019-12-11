---
title: Get-GlpiToolsDropdownsOSEditions
---

## SYNOPSIS
Function is getting OS Editions informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSEditions [-All] [<CommonParameters>]
```

### OSEditionId
```
Get-GlpiToolsDropdownsOSEditions -OSEditionId <String[]> [-Raw] [<CommonParameters>]
```

### OSEditionName
```
Get-GlpiToolsDropdownsOSEditions -OSEditionName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSEditionId which you can find in GLPI website
Returns object with property's of OS Editions

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSEditions -All
```

Example will return all OS Editions from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSEditions
```

Function gets OSEditionId from GLPI from Pipline, and return OS Editions object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSEditions
```

Function gets OSEditionId from GLPI from Pipline (u can pass many ID's like that), and return OS Editions object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSEditions -OSEditionId 326
```

Function gets OSEditionId from GLPI which is provided through -OSEditionId after Function type, and return OS Editions object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSEditions -OSEditionId 326, 321
```

Function gets OS EditionsId from GLPI which is provided through -OSEditionId keyword after Function type (u can provide many ID's like that), and return OS Editions object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSEditions -OSEditionName Fusion
```

Example will return glpi OS Editions, but what is the most important, OS Editions will be shown exactly as you see in glpi dropdown OS Editions.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all OS Editions from GLPI

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

### -OSEditionId
This parameter can take pipline input, either, you can use this function with -OSEditionId keyword.
Provide to this param OSEditionId from GLPI OS Editions Bookmark

```yaml
Type: String[]
Parameter Sets: OSEditionId
Aliases: OSEID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSEditionId Parameter.
OSEditionId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSEditionId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSEditionName
This parameter can take pipline input, either, you can use this function with -OSEditionId keyword.
Provide to this param OS Editions Name from GLPI OS Editions Bookmark

```yaml
Type: String
Parameter Sets: OSEditionName
Aliases: OSEN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### OS Editions ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of OS Editions from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
