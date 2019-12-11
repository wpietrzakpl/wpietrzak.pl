---
title: Get-GlpiToolsDataCenters
---

## SYNOPSIS
Function is getting Data Center informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDataCenters [-All] [<CommonParameters>]
```

### DataCenterId
```
Get-GlpiToolsDataCenters -DataCenterId <String[]> [-Raw] [<CommonParameters>]
```

### DataCenterName
```
Get-GlpiToolsDataCenters -DataCenterName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DataCenterId which you can find in GLPI website
Returns object with property's of Data Center

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDataCenters -All
```

Example will return all Data Center from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDataCenters
```

Function gets DataCenterId from GLPI from PipData Center, and return Data Center object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDataCenters
```

Function gets DataCenterId from GLPI from PipData Center (u can pass many ID's like that), and return Data Center object

### EXAMPLE 4
```
Get-GlpiToolsDataCenters -DataCenterId 326
```

Function gets DataCenterId from GLPI which is provided through -DataCenterId after Function type, and return Data Center object

### EXAMPLE 5
```
Get-GlpiToolsDataCenters -DataCenterId 326, 321
```

Function gets Data Center Id from GLPI which is provided through -DataCenterId keyword after Function type (u can provide many ID's like that), and return Data Center object

### EXAMPLE 6
```
Get-GlpiToolsDataCenters -DataCenterName Fusion
```

Example will return glpi Data Center, but what is the most important, Data Center will be shown exactly as you see in glpi dropdown Data Center.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Data Center from GLPI

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

### -DataCenterId
This parameter can take pipData Center input, either, you can use this function with -DataCenterId keyword.
Provide to this param DataCenterId from GLPI Data Center Bookmark

```yaml
Type: String[]
Parameter Sets: DataCenterId
Aliases: DCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DataCenterId Parameter.
DataCenterId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DataCenterId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataCenterName
This parameter can take pipData Center input, either, you can use this function with -DataCenterId keyword.
Provide to this param Data Center Name from GLPI Data Center Bookmark

```yaml
Type: String
Parameter Sets: DataCenterName
Aliases: DCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Data Center ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Data Center from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
