---
title: Get-GlpiToolsDropdownsThirdPartyTypes
---

## SYNOPSIS
Function is getting Third Party Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsThirdPartyTypes [-All] [<CommonParameters>]
```

### ThirdPartyTypeId
```
Get-GlpiToolsDropdownsThirdPartyTypes -ThirdPartyTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ThirdPartyTypeName
```
Get-GlpiToolsDropdownsThirdPartyTypes -ThirdPartyTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ThirdPartyTypeId which you can find in GLPI website
Returns object with property's of Third Party Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsThirdPartyTypes -All
```

Example will return all Third Party Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsThirdPartyTypes
```

Function gets ThirdPartyTypeId from GLPI from Pipline, and return Third Party Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsThirdPartyTypes
```

Function gets ThirdPartyTypeId from GLPI from Pipline (u can pass many ID's like that), and return Third Party Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsThirdPartyTypes -ThirdPartyTypeId 326
```

Function gets ThirdPartyTypeId from GLPI which is provided through -ThirdPartyTypeId after Function type, and return Third Party Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsThirdPartyTypes -ThirdPartyTypeId 326, 321
```

Function gets Third Party Types Id from GLPI which is provided through -ThirdPartyTypeId keyword after Function type (u can provide many ID's like that), and return Third Party Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsThirdPartyTypes -ThirdPartyTypeName Fusion
```

Example will return glpi Third Party Types, but what is the most important, Third Party Types will be shown exactly as you see in glpi dropdown Third Party Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Third Party Types from GLPI

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

### -ThirdPartyTypeId
This parameter can take pipline input, either, you can use this function with -ThirdPartyTypeId keyword.
Provide to this param ThirdPartyTypeId from GLPI Third Party Types Bookmark

```yaml
Type: String[]
Parameter Sets: ThirdPartyTypeId
Aliases: TPTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ThirdPartyTypeId Parameter.
ThirdPartyTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ThirdPartyTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThirdPartyTypeName
This parameter can take pipline input, either, you can use this function with -ThirdPartyTypeId keyword.
Provide to this param Third Party Types Name from GLPI Third Party Types Bookmark

```yaml
Type: String
Parameter Sets: ThirdPartyTypeName
Aliases: TPTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Third Party Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Third Party Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
