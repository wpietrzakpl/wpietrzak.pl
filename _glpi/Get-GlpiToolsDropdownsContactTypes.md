---
title: Get-GlpiToolsDropdownsContactTypes
---

## SYNOPSIS
Function is getting Contact Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsContactTypes [-All] [<CommonParameters>]
```

### ContactTypeId
```
Get-GlpiToolsDropdownsContactTypes -ContactTypeId <String[]> [-Raw] [<CommonParameters>]
```

### ContactTypeName
```
Get-GlpiToolsDropdownsContactTypes -ContactTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ContactTypeId which you can find in GLPI website
Returns object with property's of Contact Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsContactTypes -All
```

Example will return all Contact Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsContactTypes
```

Function gets ContactTypeId from GLPI from Pipline, and return Contact Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsContactTypes
```

Function gets ContactTypeId from GLPI from Pipline (u can pass many ID's like that), and return Contact Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsContactTypes -ContactTypeId 326
```

Function gets ContactTypeId from GLPI which is provided through -ContactTypeId after Function type, and return Contact Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsContactTypes -ContactTypeId 326, 321
```

Function gets Contact Types Id from GLPI which is provided through -ContactTypeId keyword after Function type (u can provide many ID's like that), and return Contact Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsContactTypes -ContactTypeName Fusion
```

Example will return glpi Contact Types, but what is the most important, Contact Types will be shown exactly as you see in glpi dropdown Contact Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Contact Types from GLPI

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

### -ContactTypeId
This parameter can take pipline input, either, you can use this function with -ContactTypeId keyword.
Provide to this param ContactTypeId from GLPI Contact Types Bookmark

```yaml
Type: String[]
Parameter Sets: ContactTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ContactTypeId Parameter.
ContactTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ContactTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactTypeName
This parameter can take pipline input, either, you can use this function with -ContactTypeId keyword.
Provide to this param Contact Types Name from GLPI Contact Types Bookmark

```yaml
Type: String
Parameter Sets: ContactTypeName
Aliases: CTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Contact Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Contact Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
