---
title: Get-GlpiToolsDropdownsTaskCategories
---

## SYNOPSIS
Function is getting Task Categories informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsTaskCategories [-All] [<CommonParameters>]
```

### TaskCategoryId
```
Get-GlpiToolsDropdownsTaskCategories -TaskCategoryId <String[]> [-Raw] [<CommonParameters>]
```

### TaskCategoryName
```
Get-GlpiToolsDropdownsTaskCategories -TaskCategoryName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on TaskCategoryId which you can find in GLPI website
Returns object with property's of Task Categories

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsTaskCategories -All
```

Example will return all Task Categories from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsTaskCategories
```

Function gets TaskCategoryId from GLPI from Pipline, and return Task Categories object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsTaskCategories
```

Function gets TaskCategoryId from GLPI from Pipline (u can pass many ID's like that), and return Task Categories object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsTaskCategories -TaskCategoryId 326
```

Function gets TaskCategoryId from GLPI which is provided through -TaskCategoryId after Function type, and return Task Categories object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsTaskCategories -TaskCategoryId 326, 321
```

Function gets Task Categories Id from GLPI which is provided through -TaskCategoryId keyword after Function type (u can provide many ID's like that), and return Task Categories object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsTaskCategories -TaskCategoryName Fusion
```

Example will return glpi Task Categories, but what is the most important, Task Categories will be shown exactly as you see in glpi dropdown Task Categories.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Task Categories from GLPI

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

### -TaskCategoryId
This parameter can take pipline input, either, you can use this function with -TaskCategoryId keyword.
Provide to this param TaskCategoryId from GLPI Task Categories Bookmark

```yaml
Type: String[]
Parameter Sets: TaskCategoryId
Aliases: TCID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with TaskCategoryId Parameter.
TaskCategoryId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: TaskCategoryId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -TaskCategoryName
This parameter can take pipline input, either, you can use this function with -TaskCategoryId keyword.
Provide to this param Task Categories Name from GLPI Task Categories Bookmark

```yaml
Type: String
Parameter Sets: TaskCategoryName
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

### Task Categories ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Task Categories from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
