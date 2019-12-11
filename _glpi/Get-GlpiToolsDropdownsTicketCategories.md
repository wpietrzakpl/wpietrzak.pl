---
title: Get-GlpiToolsDropdownsTicketCategories
---

## SYNOPSIS
Function is getting Ticket Categories informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsTicketCategories [-All] [<CommonParameters>]
```

### TicketCategoriesId
```
Get-GlpiToolsDropdownsTicketCategories -TicketCategoriesId <String[]> [-Raw] [<CommonParameters>]
```

### TicketCategoriesName
```
Get-GlpiToolsDropdownsTicketCategories -TicketCategoriesName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on TicketCategoriesId which you can find in GLPI website
Returns object with property's of Ticket Categories

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsTicketCategories -All
```

Example will return all Ticket Categories from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsTicketCategories
```

Function gets TicketCategoriesId from GLPI from Pipline, and return Ticket Categories object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsTicketCategories
```

Function gets TicketCategoriesId from GLPI from Pipline (u can pass many ID's like that), and return Ticket Categories object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsTicketCategories -TicketCategoriesId 326
```

Function gets TicketCategoriesId from GLPI which is provided through -TicketCategoriesId after Function type, and return Ticket Categories object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsTicketCategories -TicketCategoriesId 326, 321
```

Function gets Ticket CategoriesId from GLPI which is provided through -TicketCategoriesId keyword after Function type (u can provide many ID's like that), and return Ticket Categories object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsTicketCategories -TicketCategoriesName Fusion
```

Example will return glpi Ticket Categories, but what is the most important, Ticket Categories will be shown exactly as you see in glpi dropdown Ticket Categories.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Ticket Categories from GLPI

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

### -TicketCategoriesId
This parameter can take pipline input, either, you can use this function with -TicketCategoriesId keyword.
Provide to this param TicketCategoriesId from GLPI Ticket Categories Bookmark

```yaml
Type: String[]
Parameter Sets: TicketCategoriesId
Aliases: TCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with TicketCategoriesId Parameter.
TicketCategoriesId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: TicketCategoriesId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TicketCategoriesName
This parameter can take pipline input, either, you can use this function with -TicketCategoriesId keyword.
Provide to this param Ticket Categories Name from GLPI Ticket Categories Bookmark

```yaml
Type: String
Parameter Sets: TicketCategoriesName
Aliases: TCN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Ticket Categories ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Ticket Categories from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
