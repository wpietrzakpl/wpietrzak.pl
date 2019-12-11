---
title: Get-GlpiToolsDropdownsPduModels
---

## SYNOPSIS
Function is getting Pdu Models informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsPduModels [-All] [<CommonParameters>]
```

### PduModelId
```
Get-GlpiToolsDropdownsPduModels -PduModelId <String[]> [-Raw] [<CommonParameters>]
```

### PduModelName
```
Get-GlpiToolsDropdownsPduModels -PduModelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on PduModelId which you can find in GLPI website
Returns object with property's of Pdu Models

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsPduModels -All
```

Example will return all Pdu Models from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsPduModels
```

Function gets PduModelId from GLPI from Pipline, and return Pdu Models object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsPduModels
```

Function gets PduModelId from GLPI from Pipline (u can pass many ID's like that), and return Pdu Models object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsPduModels -PduModelId 326
```

Function gets PduModelId from GLPI which is provided through -PduModelId after Function type, and return Pdu Models object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsPduModels -PduModelId 326, 321
```

Function gets Pdu Models Id from GLPI which is provided through -PduModelId keyword after Function type (u can provide many ID's like that), and return Pdu Models object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsPduModels -PduModelName Fusion
```

Example will return glpi Pdu Models, but what is the most important, Pdu Models will be shown exactly as you see in glpi dropdown Pdu Models.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Pdu Models from GLPI

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

### -PduModelId
This parameter can take pipline input, either, you can use this function with -PduModelId keyword.
Provide to this param PduModelId from GLPI Pdu Models Bookmark

```yaml
Type: String[]
Parameter Sets: PduModelId
Aliases: PMID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with PduModelId Parameter.
PduModelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: PduModelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PduModelName
This parameter can take pipline input, either, you can use this function with -PduModelId keyword.
Provide to this param Pdu Models Name from GLPI Pdu Models Bookmark

```yaml
Type: String
Parameter Sets: PduModelName
Aliases: PMN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Pdu Models ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Pdu Models from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
