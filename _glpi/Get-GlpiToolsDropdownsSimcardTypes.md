---
title: Get-GlpiToolsDropdownsSimcardTypes
---

## SYNOPSIS
Function is getting Simcard Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsSimcardTypes [-All] [<CommonParameters>]
```

### SimcardTypeId
```
Get-GlpiToolsDropdownsSimcardTypes -SimcardTypeId <String[]> [-Raw] [<CommonParameters>]
```

### SimcardTypeName
```
Get-GlpiToolsDropdownsSimcardTypes -SimcardTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on SimcardTypeId which you can find in GLPI website
Returns object with property's of Simcard Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsSimcardTypes -All
```

Example will return all Simcard Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsSimcardTypes
```

Function gets SimcardTypeId from GLPI from Pipline, and return Simcard Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsSimcardTypes
```

Function gets SimcardTypeId from GLPI from Pipline (u can pass many ID's like that), and return Simcard Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsSimcardTypes -SimcardTypeId 326
```

Function gets SimcardTypeId from GLPI which is provided through -SimcardTypeId after Function type, and return Simcard Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsSimcardTypes -SimcardTypeId 326, 321
```

Function gets Simcard Types Id from GLPI which is provided through -SimcardTypeId keyword after Function type (u can provide many ID's like that), and return Simcard Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsSimcardTypes -SimcardTypeName Fusion
```

Example will return glpi Simcard Types, but what is the most important, Simcard Types will be shown exactly as you see in glpi dropdown Simcard Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Simcard Types from GLPI

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

### -SimcardTypeId
This parameter can take pipline input, either, you can use this function with -SimcardTypeId keyword.
Provide to this param SimcardTypeId from GLPI Simcard Types Bookmark

```yaml
Type: String[]
Parameter Sets: SimcardTypeId
Aliases: STID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SimcardTypeId Parameter.
SimcardTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SimcardTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -SimcardTypeName
This parameter can take pipline input, either, you can use this function with -SimcardTypeId keyword.
Provide to this param Simcard Types Name from GLPI Simcard Types Bookmark

```yaml
Type: String
Parameter Sets: SimcardTypeName
Aliases: STN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Simcard Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Simcard Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
