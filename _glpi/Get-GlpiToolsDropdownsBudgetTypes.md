---
title: Get-GlpiToolsDropdownsBudgetTypes
---

## SYNOPSIS
Function is getting Budget Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsBudgetTypes [-All] [<CommonParameters>]
```

### BudgetTypeId
```
Get-GlpiToolsDropdownsBudgetTypes -BudgetTypeId <String[]> [-Raw] [<CommonParameters>]
```

### BudgetTypeName
```
Get-GlpiToolsDropdownsBudgetTypes -BudgetTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on BudgetTypeId which you can find in GLPI website
Returns object with property's of Budget Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsBudgetTypes -All
```

Example will return all Budget Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsBudgetTypes
```

Function gets BudgetTypeId from GLPI from Pipline, and return Budget Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsBudgetTypes
```

Function gets BudgetTypeId from GLPI from Pipline (u can pass many ID's like that), and return Budget Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsBudgetTypes -BudgetTypeId 326
```

Function gets BudgetTypeId from GLPI which is provided through -BudgetTypeId after Function type, and return Budget Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsBudgetTypes -BudgetTypeId 326, 321
```

Function gets Budget Types Id from GLPI which is provided through -BudgetTypeId keyword after Function type (u can provide many ID's like that), and return Budget Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsBudgetTypes -BudgetTypeName Fusion
```

Example will return glpi Budget Types, but what is the most important, Budget Types will be shown exactly as you see in glpi dropdown Budget Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Budget Types from GLPI

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

### -BudgetTypeId
This parameter can take pipline input, either, you can use this function with -BudgetTypeId keyword.
Provide to this param BudgetTypeId from GLPI Budget Types Bookmark

```yaml
Type: String[]
Parameter Sets: BudgetTypeId
Aliases: BTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with BudgetTypeId Parameter.
BudgetTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: BudgetTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BudgetTypeName
This parameter can take pipline input, either, you can use this function with -BudgetTypeId keyword.
Provide to this param Budget Types Name from GLPI Budget Types Bookmark

```yaml
Type: String
Parameter Sets: BudgetTypeName
Aliases: BTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Budget Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Budget Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
