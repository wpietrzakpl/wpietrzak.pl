---
title: Get-GlpiToolsConsumableItems
---

## SYNOPSIS
Function is getting ConsumableItem informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsConsumableItems [-All] [<CommonParameters>]
```

### ConsumableItemId
```
Get-GlpiToolsConsumableItems -ConsumableItemId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### ConsumableItemName
```
Get-GlpiToolsConsumableItems -ConsumableItemName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on ConsumableItemID which you can find in GLPI website
Returns object with property's of ConsumableItem

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsConsumableItems
```

Function gets ConsumableItemID from GLPI from Pipline, and return ConsumableItem object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsConsumableItems
```

Function gets ConsumableItemID from GLPI from Pipline (u can pass many ID's like that), and return ConsumableItem object

### EXAMPLE 3
```
Get-GlpiToolsConsumableItems -ConsumableItemId 326
```

Function gets ConsumableItemID from GLPI which is provided through -ConsumableItemId after Function type, and return ConsumableItem object

### EXAMPLE 4
```
Get-GlpiToolsConsumableItems -ConsumableItemId 326, 321
```

Function gets ConsumableItemID from GLPI which is provided through -ConsumableItemId keyword after Function type (u can provide many ID's like that), and return ConsumableItem object

### EXAMPLE 5
```
Get-GlpiToolsConsumableItems -ConsumableItemId 234 -Raw
```

Example will show ConsumableItem with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsConsumableItems -Raw
```

Example will show ConsumableItem with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsConsumableItems -ConsumableItemName glpi
```

Example will return glpi ConsumableItem, but what is the most important, ConsumableItem will be shown exacly as you see in glpi ConsumableItems tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsConsumableItems -ConsumableItemName glpi -SearchInTrash Yes
```

Example will return glpi ConsumableItem, but from trash

## PARAMETERS

### -All
This parameter will return all ConsumableItems from GLPI

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

### -ConsumableItemId
This parameter can take pipline input, either, you can use this function with -ConsumableItemId keyword.
Provide to this param ConsumableItem ID from GLPI ConsumableItems Bookmark

```yaml
Type: String[]
Parameter Sets: ConsumableItemId
Aliases: CIID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ConsumableItemId Parameter.
ConsumableItemId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ConsumableItemId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConsumableItemName
Provide to this param ConsumableItem Name from GLPI ConsumableItems Bookmark

```yaml
Type: String
Parameter Sets: ConsumableItemName
Aliases: CIN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with ConsumableItemName Parameter.
If you want Search for ConsumableItem name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: ConsumableItemName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with ConsumableItemId Parameter. 
If you want to get additional parameter of ConsumableItem object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: ConsumableItemId
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

### ConsumableItem ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of ConsumableItems from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
