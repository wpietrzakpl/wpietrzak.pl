---
title: Get-GlpiToolsChanges
---

## SYNOPSIS
Function is getting Change informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsChanges [-All] [<CommonParameters>]
```

### ChangeId
```
Get-GlpiToolsChanges -ChangeId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### ChangeName
```
Get-GlpiToolsChanges -ChangeName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on ChangeID which you can find in GLPI website
Returns object with property's of Change

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsChanges
```

Function gets ChangeID from GLPI from Pipline, and return Change object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsChanges
```

Function gets ChangeID from GLPI from Pipline (u can pass many ID's like that), and return Change object

### EXAMPLE 3
```
Get-GlpiToolsChanges -ChangeId 326
```

Function gets ChangeID from GLPI which is provided through -ChangeId after Function type, and return Change object

### EXAMPLE 4
```
Get-GlpiToolsChanges -ChangeId 326, 321
```

Function gets ChangeID from GLPI which is provided through -ChangeId keyword after Function type (u can provide many ID's like that), and return Change object

### EXAMPLE 5
```
Get-GlpiToolsChanges -ChangeId 234 -Raw
```

Example will show Change with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsChanges -Raw
```

Example will show Change with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsChanges -ChangeName glpi
```

Example will return glpi Change, but what is the most important, Change will be shown exacly as you see in glpi Changes tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsChanges -ChangeName glpi -SearchInTrash Yes
```

Example will return glpi Change, but from trash

## PARAMETERS

### -All
This parameter will return all Changes from GLPI

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

### -ChangeId
This parameter can take pipline input, either, you can use this function with -ChangeId keyword.
Provide to this param Change ID from GLPI Changes Bookmark

```yaml
Type: String[]
Parameter Sets: ChangeId
Aliases: CID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ChangeId Parameter.
ChangeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ChangeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChangeName
Provide to this param Change Name from GLPI Changes Bookmark

```yaml
Type: String
Parameter Sets: ChangeName
Aliases: CN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with ChangeName Parameter.
If you want Search for Change name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: ChangeName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with ChangeId Parameter. 
If you want to get additional parameter of Change object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: ChangeId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Change ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Changes from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
