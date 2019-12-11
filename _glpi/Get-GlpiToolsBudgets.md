---
title: Get-GlpiToolsBudgets
---

## SYNOPSIS
Function is getting Budget informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsBudgets [-All] [<CommonParameters>]
```

### BudgetId
```
Get-GlpiToolsBudgets -BudgetId <String[]> [-Raw] [<CommonParameters>]
```

### BudgetName
```
Get-GlpiToolsBudgets -BudgetName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on BudgetId which you can find in GLPI website
Returns object with property's of Budget

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsBudgets -All
```

Example will return all Budget from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsBudgets
```

Function gets BudgetId from GLPI from Pipline, and return Budget object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsBudgets
```

Function gets BudgetId from GLPI from Pipline (u can pass many ID's like that), and return Budget object

### EXAMPLE 4
```
Get-GlpiToolsBudgets -BudgetId 326
```

Function gets BudgetId from GLPI which is provided through -BudgetId after Function type, and return Budget object

### EXAMPLE 5
```
Get-GlpiToolsBudgets -BudgetId 326, 321
```

Function gets Budget Id from GLPI which is provided through -BudgetId keyword after Function type (u can provide many ID's like that), and return Budget object

### EXAMPLE 6
```
Get-GlpiToolsBudgets -BudgetName Fusion
```

Example will return glpi Budget, but what is the most important, Budget will be shown exactly as you see in glpi dropdown Budget.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Budget from GLPI

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

### -BudgetId
This parameter can take pipline input, either, you can use this function with -BudgetId keyword.
Provide to this param BudgetId from GLPI Budget Bookmark

```yaml
Type: String[]
Parameter Sets: BudgetId
Aliases: BID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with BudgetId Parameter.
BudgetId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: BudgetId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BudgetName
This parameter can take pipline input, either, you can use this function with -BudgetId keyword.
Provide to this param Budget Name from GLPI Budget Bookmark

```yaml
Type: String
Parameter Sets: BudgetName
Aliases: BN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Budget ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Budget from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
