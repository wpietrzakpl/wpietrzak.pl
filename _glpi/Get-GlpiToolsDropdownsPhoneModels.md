---
title: Get-GlpiToolsDropdownsPhoneModels
---

## SYNOPSIS
Function is getting Phone Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPhoneModels [-All] [<CommonParameters>]
```

### PhoneModelId
```
Get-GlpiToolsDropdownsPhoneModels -PhoneModelId <String[]> [-Raw] [<CommonParameters>]
```

### PhonelModelName
```
Get-GlpiToolsDropdownsPhoneModels -PhoneModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PhoneModelId which you can find in GLPI website
Returns object with property's of Phone Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPhoneModels -All
```

Example will return all Phone Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPhoneModels
```

Function gets PhoneModelId from GLPI from Pipline, and return Phone Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPhoneModels
```

Function gets PhoneModelId from GLPI from Pipline (u can pass many ID's like that), and return Phone Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPhoneModels -PhoneModelId 326
```

Function gets PhoneModelId from GLPI which is provided through -PhoneModelId after Function type, and return Phone Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPhoneModels -PhoneModelId 326, 321
```

Function gets Phone Models Id from GLPI which is provided through -PhoneModelId keyword after Function type (u can provide many ID's like that), and return Phone Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPhoneModels -PhoneModelName Fusion
```

Example will return glpi Phone Models, but what is the most important, Phone Models will be shown exactly as you see in glpi dropdown Phone Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Phone Models from GLPI

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

### -PhoneModelId
This parameter can take pipline input, either, you can use this function with -PhoneModelId keyword.
Provide to this param PhoneModelId from GLPI Phone Models Bookmark

```yaml
Type: String[]
Parameter Sets: PhoneModelId
Aliases: PMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PhoneModelId Parameter.
PhoneModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PhoneModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PhoneModelName
This parameter can take pipline input, either, you can use this function with -PhoneModelId keyword.
Provide to this param Phone Models Name from GLPI Phone Models Bookmark

```yaml
Type: String
Parameter Sets: PhonelModelName
Aliases: PMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Phone Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Phone Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
