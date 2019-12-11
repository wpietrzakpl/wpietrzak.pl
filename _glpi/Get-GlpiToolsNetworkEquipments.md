---
title: Get-GlpiToolsNetworkEquipments
---

## SYNOPSIS
Function is getting NetworkEquipment informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsNetworkEquipments [-All] [<CommonParameters>]
```

### NetworkEquipmentId
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### NetworkEquipmentName
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on NetworkEquipmentID which you can find in GLPI website
Returns object with property's of NetworkEquipment

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsNetworkEquipments
```

Function gets NetworkEquipmentID from GLPI from Pipline, and return NetworkEquipment object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsNetworkEquipments
```

Function gets NetworkEquipmentID from GLPI from Pipline (u can pass many ID's like that), and return NetworkEquipment object

### EXAMPLE 3
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentId 326
```

Function gets NetworkEquipmentID from GLPI which is provided through -NetworkEquipmentId after Function type, and return NetworkEquipment object

### EXAMPLE 4
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentId 326, 321
```

Function gets NetworkEquipmentID from GLPI which is provided through -NetworkEquipmentId keyword after Function type (u can provide many ID's like that), and return NetworkEquipment object

### EXAMPLE 5
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentId 234 -Raw
```

Example will show NetworkEquipment with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsNetworkEquipments -Raw
```

Example will show NetworkEquipment with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentName glpi
```

Example will return glpi NetworkEquipment, but what is the most important, NetworkEquipment will be shown exacly as you see in glpi NetworkEquipments tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsNetworkEquipments -NetworkEquipmentName glpi -SearchInTrash Yes
```

Example will return glpi NetworkEquipment, but from trash

## PARAMETERS

### -All
This parameter will return all NetworkEquipments from GLPI

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

### -NetworkEquipmentId
This parameter can take pipline input, either, you can use this function with -NetworkEquipmentId keyword.
Provide to this param NetworkEquipment ID from GLPI NetworkEquipments Bookmark

```yaml
Type: String[]
Parameter Sets: NetworkEquipmentId
Aliases: MID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with NetworkEquipmentId Parameter.
NetworkEquipmentId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: NetworkEquipmentId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkEquipmentName
Provide to this param NetworkEquipment Name from GLPI NetworkEquipments Bookmark

```yaml
Type: String
Parameter Sets: NetworkEquipmentName
Aliases: NEN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with NetworkEquipmentName Parameter.
If you want Search for NetworkEquipment name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: NetworkEquipmentName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with NetworkEquipmentId Parameter. 
If you want to get additional parameter of NetworkEquipment object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: NetworkEquipmentId
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

### NetworkEquipment ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of NetworkEquipments from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
