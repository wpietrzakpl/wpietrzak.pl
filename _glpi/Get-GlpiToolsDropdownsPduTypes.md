---
title: Get-GlpiToolsDropdownsPduTypes
---

## SYNOPSIS
Function is getting Pdu Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPduTypes [-All] [<CommonParameters>]
```

### PduTypeId
```
Get-GlpiToolsDropdownsPduTypes -PduTypeId <String[]> [-Raw] [<CommonParameters>]
```

### PduTypeName
```
Get-GlpiToolsDropdownsPduTypes -PduTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PduTypeId which you can find in GLPI website
Returns object with property's of Pdu Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPduTypes -All
```

Example will return all Pdu Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPduTypes
```

Function gets PduTypeId from GLPI from Pipline, and return Pdu Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPduTypes
```

Function gets PduTypeId from GLPI from Pipline (u can pass many ID's like that), and return Pdu Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPduTypes -PduTypeId 326
```

Function gets PduTypeId from GLPI which is provided through -PduTypeId after Function type, and return Pdu Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPduTypes -PduTypeId 326, 321
```

Function gets Pdu Types Id from GLPI which is provided through -PduTypeId keyword after Function type (u can provide many ID's like that), and return Pdu Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPduTypes -PduTypeName Fusion
```

Example will return glpi Pdu Types, but what is the most important, Pdu Types will be shown exactly as you see in glpi dropdown Pdu Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Pdu Types from GLPI

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

### -PduTypeId
This parameter can take pipline input, either, you can use this function with -PduTypeId keyword.
Provide to this param PduTypeId from GLPI Pdu Types Bookmark

```yaml
Type: String[]
Parameter Sets: PduTypeId
Aliases: PTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PduTypeId Parameter.
PduTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PduTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PduTypeName
This parameter can take pipline input, either, you can use this function with -PduTypeId keyword.
Provide to this param Pdu Types Name from GLPI Pdu Types Bookmark

```yaml
Type: String
Parameter Sets: PduTypeName
Aliases: PTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Pdu Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Pdu Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
