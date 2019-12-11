---
title: Get-GlpiToolsDropdownsPhonesPowerSupplyTypes
---

## SYNOPSIS
Function is getting Phones Power Supply Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes [-All] [<CommonParameters>]
```

### PhonePowerSupplyTypeId
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -PhonePowerSupplyTypeId <String[]> [-Raw] [<CommonParameters>]
```

### PhonePowerSupplyTypeName
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -PhonePowerSupplyTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PhonePowerSupplyTypeId which you can find in GLPI website
Returns object with property's of Phones Power Supply Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -All
```

Example will return all Phones Power Supply Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPhonesPowerSupplyTypes
```

Function gets PhonePowerSupplyTypeId from GLPI from Pipline, and return Phones Power Supply Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPhonesPowerSupplyTypes
```

Function gets PhonePowerSupplyTypeId from GLPI from Pipline (u can pass many ID's like that), and return Phones Power Supply Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -PhonePowerSupplyTypeId 326
```

Function gets PhonePowerSupplyTypeId from GLPI which is provided through -PhonePowerSupplyTypeId after Function type, and return Phones Power Supply Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -PhonePowerSupplyTypeId 326, 321
```

Function gets Phones Power Supply Types Id from GLPI which is provided through -PhonePowerSupplyTypeId keyword after Function type (u can provide many ID's like that), and return Phones Power Supply Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPhonesPowerSupplyTypes -PhonePowerSupplyTypeName Fusion
```

Example will return glpi Phones Power Supply Types, but what is the most important, Phones Power Supply Types will be shown exactly as you see in glpi dropdown Phones Power Supply Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Phones Power Supply Types from GLPI

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

### -PhonePowerSupplyTypeId
This parameter can take pipline input, either, you can use this function with -PhonePowerSupplyTypeId keyword.
Provide to this param PhonePowerSupplyTypeId from GLPI Phones Power Supply Types Bookmark

```yaml
Type: String[]
Parameter Sets: PhonePowerSupplyTypeId
Aliases: PPSTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PhonePowerSupplyTypeId Parameter.
PhonePowerSupplyTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PhonePowerSupplyTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PhonePowerSupplyTypeName
This parameter can take pipline input, either, you can use this function with -PhonePowerSupplyTypeId keyword.
Provide to this param Phones Power Supply Types Name from GLPI Phones Power Supply Types Bookmark

```yaml
Type: String
Parameter Sets: PhonePowerSupplyTypeName
Aliases: PPSTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Phones Power Supply Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Phones Power Supply Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
