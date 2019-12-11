---
title: Get-GlpiToolsDropdownsBussinessCriticities
---

## SYNOPSIS
Function is getting Bussiness Criticities informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsBussinessCriticities [-All] [<CommonParameters>]
```

### BussinessCriticityId
```
Get-GlpiToolsDropdownsBussinessCriticities -BussinessCriticityId <String[]> [-Raw] [<CommonParameters>]
```

### BussinessCriticityName
```
Get-GlpiToolsDropdownsBussinessCriticities -BussinessCriticityName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on BussinessCriticityId which you can find in GLPI website
Returns object with property's of Bussiness Criticities

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsBussinessCriticities -All
```

Example will return all Bussiness Criticities from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsBussinessCriticities
```

Function gets BussinessCriticityId from GLPI from pipeline, and return Bussiness Criticities object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsBussinessCriticities
```

Function gets BussinessCriticityId from GLPI from pipeline (u can pass many ID's like that), and return Bussiness Criticities object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsBussinessCriticities -BussinessCriticityId 326
```

Function gets BussinessCriticityId from GLPI which is provided through -BussinessCriticityId after Function type, and return Bussiness Criticities object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsBussinessCriticities -BussinessCriticityId 326, 321
```

Function gets Bussiness Criticities Id from GLPI which is provided through -BussinessCriticityId keyword after Function type (u can provide many ID's like that), and return Bussiness Criticities object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsBussinessCriticities -BussinessCriticityName Fusion
```

Example will return glpi Bussiness Criticities, but what is the most important, Bussiness Criticities will be shown exactly as you see in glpi dropdown Bussiness Criticities.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Bussiness Criticities from GLPI

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

### -BussinessCriticityId
This parameter can take pipeline input, either, you can use this function with -BussinessCriticityId keyword.
Provide to this param BussinessCriticityId from GLPI Bussiness Criticities Bookmark

```yaml
Type: String[]
Parameter Sets: BussinessCriticityId
Aliases: BCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with BussinessCriticityId Parameter.
BussinessCriticityId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: BussinessCriticityId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BussinessCriticityName
This parameter can take pipeline input, either, you can use this function with -BussinessCriticityId keyword.
Provide to this param Bussiness Criticities Name from GLPI Bussiness Criticities Bookmark

```yaml
Type: String
Parameter Sets: BussinessCriticityName
Aliases: BCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Bussiness Criticities ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Bussiness Criticities from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
