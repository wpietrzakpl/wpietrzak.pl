---
title: Get-GlpiToolsDropdownsGenericDeviceTypes
---

## SYNOPSIS
Function is getting Generic Device Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsGenericDeviceTypes [-All] [<CommonParameters>]
```

### GenericDeviceTypeId
```
Get-GlpiToolsDropdownsGenericDeviceTypes -GenericDeviceTypeId <String[]> [-Raw] [<CommonParameters>]
```

### GenericDeviceTypeName
```
Get-GlpiToolsDropdownsGenericDeviceTypes -GenericDeviceTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on GenericDeviceTypeId which you can find in GLPI website
Returns object with property's of Generic Device Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsGenericDeviceTypes -All
```

Example will return all Generic Device Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsGenericDeviceTypes
```

Function gets GenericDeviceTypeId from GLPI from Pipline, and return Generic Device Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsGenericDeviceTypes
```

Function gets GenericDeviceTypeId from GLPI from Pipline (u can pass many ID's like that), and return Generic Device Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsGenericDeviceTypes -GenericDeviceTypeId 326
```

Function gets GenericDeviceTypeId from GLPI which is provided through -GenericDeviceTypeId after Function type, and return Generic Device Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsGenericDeviceTypes -GenericDeviceTypeId 326, 321
```

Function gets Generic Device Types Id from GLPI which is provided through -GenericDeviceTypeId keyword after Function type (u can provide many ID's like that), and return Generic Device Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsGenericDeviceTypes -GenericDeviceTypeName Fusion
```

Example will return glpi Generic Device Types, but what is the most important, Generic Device Types will be shown exactly as you see in glpi dropdown Generic Device Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Generic Device Types from GLPI

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

### -GenericDeviceTypeId
This parameter can take pipline input, either, you can use this function with -GenericDeviceTypeId keyword.
Provide to this param GenericDeviceTypeId from GLPI Generic Device Types Bookmark

```yaml
Type: String[]
Parameter Sets: GenericDeviceTypeId
Aliases: GDTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with GenericDeviceTypeId Parameter.
GenericDeviceTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: GenericDeviceTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -GenericDeviceTypeName
This parameter can take pipline input, either, you can use this function with -GenericDeviceTypeId keyword.
Provide to this param Generic Device Types Name from GLPI Generic Device Types Bookmark

```yaml
Type: String
Parameter Sets: GenericDeviceTypeName
Aliases: GDTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Generic Device Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Generic Device Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
