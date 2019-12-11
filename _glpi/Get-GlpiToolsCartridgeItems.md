---
title: Get-GlpiToolsCartridgeItems
---

## SYNOPSIS
Function is getting CartridgeItem informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsCartridgeItems [-All] [<CommonParameters>]
```

### CartridgeItemId
```
Get-GlpiToolsCartridgeItems -CartridgeItemId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### CartridgeItemName
```
Get-GlpiToolsCartridgeItems -CartridgeItemName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on CartridgeItemID which you can find in GLPI website
Returns object with property's of CartridgeItem

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsCartridgeItems
```

Function gets CartridgeItemID from GLPI from Pipline, and return CartridgeItem object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsCartridgeItems
```

Function gets CartridgeItemID from GLPI from Pipline (u can pass many ID's like that), and return CartridgeItem object

### EXAMPLE 3
```
Get-GlpiToolsCartridgeItems -CartridgeItemId 326
```

Function gets CartridgeItemID from GLPI which is provided through -CartridgeItemId after Function type, and return CartridgeItem object

### EXAMPLE 4
```
Get-GlpiToolsCartridgeItems -CartridgeItemId 326, 321
```

Function gets CartridgeItemID from GLPI which is provided through -CartridgeItemId keyword after Function type (u can provide many ID's like that), and return CartridgeItem object

### EXAMPLE 5
```
Get-GlpiToolsCartridgeItems -CartridgeItemId 234 -Raw
```

Example will show CartridgeItem with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsCartridgeItems -Raw
```

Example will show CartridgeItem with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsCartridgeItems -CartridgeItemName glpi
```

Example will return glpi CartridgeItem, but what is the most important, CartridgeItem will be shown exacly as you see in glpi CartridgeItems tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsCartridgeItems -CartridgeItemName glpi -SearchInTrash Yes
```

Example will return glpi CartridgeItem, but from trash

## PARAMETERS

### -All
This parameter will return all CartridgeItems from GLPI

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

### -CartridgeItemId
This parameter can take pipline input, either, you can use this function with -CartridgeItemId keyword.
Provide to this param CartridgeItem ID from GLPI CartridgeItems Bookmark

```yaml
Type: String[]
Parameter Sets: CartridgeItemId
Aliases: CIID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with CartridgeItemId Parameter.
CartridgeItemId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: CartridgeItemId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CartridgeItemName
Provide to this param CartridgeItem Name from GLPI CartridgeItems Bookmark

```yaml
Type: String
Parameter Sets: CartridgeItemName
Aliases: CIN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with CartridgeItemName Parameter.
If you want Search for CartridgeItem name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: CartridgeItemName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with CartridgeItemId Parameter. 
If you want to get additional parameter of CartridgeItem object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: CartridgeItemId
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

### CartridgeItem ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of CartridgeItems from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
