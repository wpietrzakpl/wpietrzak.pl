---
title: Get-GlpiToolsDropdownsLocations
---

## SYNOPSIS
Function is getting Locations informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsLocations [-All] [<CommonParameters>]
```

### LocationsId
```
Get-GlpiToolsDropdownsLocations -LocationsId <String[]> [-Raw] [<CommonParameters>]
```

### LocationsName
```
Get-GlpiToolsDropdownsLocations -LocationsName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on LocationsID which you can find in GLPI website
Returns object with property's of Locations

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsLocations -All
```

Example will return all Locations from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsLocations
```

Function gets LocationsId from GLPI from Pipline, and return Locations object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsLocations
```

Function gets LocationsId from GLPI from Pipline (u can pass many ID's like that), and return Locations object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsLocations -LocationsId 326
```

Function gets LocationsId from GLPI which is provided through -LocationsId after Function type, and return Locations object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsLocations -LocationsId 326, 321
```

Function gets LocationsId from GLPI which is provided through -LocationsId keyword after Function type (u can provide many ID's like that), and return Locations object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsLocations -LocationsName Fusion
```

Example will return glpi location, but what is the most important, location will be shown exactly as you see in glpi dropdown Locations.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Locations from GLPI

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

### -LocationsId
This parameter can take pipline input, either, you can use this function with -LocationsId keyword.
Provide to this param Locations ID from GLPI Locations Bookmark

```yaml
Type: String[]
Parameter Sets: LocationsId
Aliases: LID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with LocationsId Parameter.
LocationsId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: LocationsId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocationsName
This parameter can take pipline input, either, you can use this function with -LocationsName keyword.
Provide to this param Locations Name from GLPI Locations Bookmark

```yaml
Type: String
Parameter Sets: LocationsName
Aliases: LN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Locations ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Locations from GLPI
## NOTES
PSP 06/2019

## RELATED LINKS
