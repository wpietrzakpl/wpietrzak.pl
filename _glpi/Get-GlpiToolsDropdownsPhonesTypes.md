---
title: Get-GlpiToolsDropdownsPhonesTypes
---

## SYNOPSIS
Function is getting Phones Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPhonesTypes [-All] [<CommonParameters>]
```

### PhoneTypeId
```
Get-GlpiToolsDropdownsPhonesTypes -PhoneTypeId <String[]> [-Raw] [<CommonParameters>]
```

### PhoneTypeName
```
Get-GlpiToolsDropdownsPhonesTypes -PhoneTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PhoneTypeId which you can find in GLPI website
Returns object with property's of Phones Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPhonesTypes -All
```

Example will return all Phones Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPhonesTypes
```

Function gets PhoneTypeId from GLPI from Pipline, and return Phones Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPhonesTypes
```

Function gets PhoneTypeId from GLPI from Pipline (u can pass many ID's like that), and return Phones Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPhonesTypes -PhoneTypeId 326
```

Function gets PhoneTypeId from GLPI which is provided through -PhoneTypeId after Function type, and return Phones Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPhonesTypes -PhoneTypeId 326, 321
```

Function gets Phones Types Id from GLPI which is provided through -PhoneTypeId keyword after Function type (u can provide many ID's like that), and return Phones Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPhonesTypes -PhoneTypeName Fusion
```

Example will return glpi Phones Types, but what is the most important, Phones Types will be shown exactly as you see in glpi dropdown Phones Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Phones Types from GLPI

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

### -PhoneTypeId
This parameter can take pipline input, either, you can use this function with -PhoneTypeId keyword.
Provide to this param PhoneTypeId from GLPI Phones Types Bookmark

```yaml
Type: String[]
Parameter Sets: PhoneTypeId
Aliases: PTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PhoneTypeId Parameter.
PhoneTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PhoneTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PhoneTypeName
This parameter can take pipline input, either, you can use this function with -PhoneTypeId keyword.
Provide to this param Phones Types Name from GLPI Phones Types Bookmark

```yaml
Type: String
Parameter Sets: PhoneTypeName
Aliases: PTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Phones Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Phones Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
