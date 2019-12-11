---
title: Get-GlpiToolsDropdownsStatusesOfItems
---

## SYNOPSIS
Function gets statuses of items

## SYNTAX

### All
```
Get-GlpiToolsDropdownsStatusesOfItems [-All] [<CommonParameters>]
```

### StatesId
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesId <String[]> [-Raw] [<CommonParameters>]
```

### StatesName
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesName <String> [<CommonParameters>]
```

## DESCRIPTION
Function gets statuses of items which can be defined in dropowns

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsStatusesOfItems -All
```

Example will return all States from States.

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsStatusesOfItems
```

Function gets StatesID from GLPI from Pipline, and return States object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsStatusesOfItems
```

Function gets StatesID from GLPI from Pipline (u can pass many ID's like that), and return States object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesId 326
```

Function gets StatesID from GLPI which is provided through -StatesId after Function type, and return States object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesId 326, 321
```

Function gets StatesID from GLPI which is provided through -StatesId keyword after Function type (u can provide many ID's like that), and return States object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesId 234 -Raw
```

Example will show States with id 234, but without any parameter converted

### EXAMPLE 7
```
234 | Get-GlpiToolsDropdownsStatusesOfItems -Raw
```

Example will show States with id 234, but without any parameter converted

### EXAMPLE 8
```
Get-GlpiToolsDropdownsStatusesOfItems -StatesName glpi
```

Example will return glpi States, but what is the most important, States will be shown exactly as you see in glpi Statuses of items tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all States from GLPI

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

### -StatesId
This parameter can take pipline input, either, you can use this function with -StatesId keyword.
Provide to this param States ID from GLPI Statuses of items Bookmark

```yaml
Type: String[]
Parameter Sets: StatesId
Aliases: SID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with StatesId Parameter.
StatesId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: StatesId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -StatesName
Provide to this param States Name from GLPI States Bookmark

```yaml
Type: String
Parameter Sets: StatesName
Aliases: SN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### StateId, StateName
## OUTPUTS

### Function returns PSCustomObject with statuses of items from GLPI
## NOTES
PSP 01/2019

## RELATED LINKS
