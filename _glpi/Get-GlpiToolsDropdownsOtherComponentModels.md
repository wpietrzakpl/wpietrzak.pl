---
title: Get-GlpiToolsDropdownsOtherComponentModels
---

## SYNOPSIS
Function is getting Other Component Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOtherComponentModels [-All] [<CommonParameters>]
```

### OtherComponentModelId
```
Get-GlpiToolsDropdownsOtherComponentModels -OtherComponentModelId <String[]> [-Raw] [<CommonParameters>]
```

### OtherComponentModelName
```
Get-GlpiToolsDropdownsOtherComponentModels -OtherComponentModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OtherComponentModelId which you can find in GLPI website
Returns object with property's of Other Component Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOtherComponentModels -All
```

Example will return all Other Component Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOtherComponentModels
```

Function gets OtherComponentModelId from GLPI from Pipline, and return Other Component Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOtherComponentModels
```

Function gets OtherComponentModelId from GLPI from Pipline (u can pass many ID's like that), and return Other Component Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOtherComponentModels -OtherComponentModelId 326
```

Function gets OtherComponentModelId from GLPI which is provided through -OtherComponentModelId after Function type, and return Other Component Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOtherComponentModels -OtherComponentModelId 326, 321
```

Function gets Other Component Models Id from GLPI which is provided through -OtherComponentModelId keyword after Function type (u can provide many ID's like that), and return Other Component Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOtherComponentModels -OtherComponentModelName Fusion
```

Example will return glpi Other Component Models, but what is the most important, Other Component Models will be shown exactly as you see in glpi dropdown Other Component Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Other Component Models from GLPI

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

### -OtherComponentModelId
This parameter can take pipline input, either, you can use this function with -OtherComponentModelId keyword.
Provide to this param OtherComponentModelId from GLPI Other Component Models Bookmark

```yaml
Type: String[]
Parameter Sets: OtherComponentModelId
Aliases: OCMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OtherComponentModelId Parameter.
OtherComponentModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OtherComponentModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OtherComponentModelName
This parameter can take pipline input, either, you can use this function with -OtherComponentModelId keyword.
Provide to this param Other Component Models Name from GLPI Other Component Models Bookmark

```yaml
Type: String
Parameter Sets: OtherComponentModelName
Aliases: OCMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Other Component Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Other Component Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
