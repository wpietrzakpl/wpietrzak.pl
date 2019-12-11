---
title: Get-GlpiToolsDropdownsCaseTypes
---

## SYNOPSIS
Function is getting Case Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsCaseTypes [-All] [<CommonParameters>]
```

### CaseTypeId
```
Get-GlpiToolsDropdownsCaseTypes -CaseTypeId <String[]> [-Raw] [<CommonParameters>]
```

### CaseTypeName
```
Get-GlpiToolsDropdownsCaseTypes -CaseTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on CaseTypeId which you can find in GLPI website
Returns object with property's of Case Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsCaseTypes -All
```

Example will return all Case Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsCaseTypes
```

Function gets CaseTypeId from GLPI from Pipline, and return Case Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsCaseTypes
```

Function gets CaseTypeId from GLPI from Pipline (u can pass many ID's like that), and return Case Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsCaseTypes -CaseTypeId 326
```

Function gets CaseTypeId from GLPI which is provided through -CaseTypeId after Function type, and return Case Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsCaseTypes -CaseTypeId 326, 321
```

Function gets Case Types Id from GLPI which is provided through -CaseTypeId keyword after Function type (u can provide many ID's like that), and return Case Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsCaseTypes -CaseTypeName Fusion
```

Example will return glpi Case Types, but what is the most important, Case Types will be shown exactly as you see in glpi dropdown Case Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Case Types from GLPI

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

### -CaseTypeId
This parameter can take pipline input, either, you can use this function with -CaseTypeId keyword.
Provide to this param CaseTypeId from GLPI Case Types Bookmark

```yaml
Type: String[]
Parameter Sets: CaseTypeId
Aliases: CTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CaseTypeId Parameter.
CaseTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CaseTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CaseTypeName
This parameter can take pipline input, either, you can use this function with -CaseTypeId keyword.
Provide to this param Case Types Name from GLPI Case Types Bookmark

```yaml
Type: String
Parameter Sets: CaseTypeName
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

### Case Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Case Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
