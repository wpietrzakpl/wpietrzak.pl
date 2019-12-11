---
title: Get-GlpiToolsDropdownsMemoryTypes
---

## SYNOPSIS
Function is getting Memory Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsMemoryTypes [-All] [<CommonParameters>]
```

### MemoryTypeId
```
Get-GlpiToolsDropdownsMemoryTypes -MemoryTypeId <String[]> [-Raw] [<CommonParameters>]
```

### MemoryTypeName
```
Get-GlpiToolsDropdownsMemoryTypes -MemoryTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on MemoryTypeId which you can find in GLPI website
Returns object with property's of Memory Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsMemoryTypes -All
```

Example will return all Memory Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsMemoryTypes
```

Function gets MemoryTypeId from GLPI from Pipline, and return Memory Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsMemoryTypes
```

Function gets MemoryTypeId from GLPI from Pipline (u can pass many ID's like that), and return Memory Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsMemoryTypes -MemoryTypeId 326
```

Function gets MemoryTypeId from GLPI which is provided through -MemoryTypeId after Function type, and return Memory Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsMemoryTypes -MemoryTypeId 326, 321
```

Function gets Memory Types Id from GLPI which is provided through -MemoryTypeId keyword after Function type (u can provide many ID's like that), and return Memory Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsMemoryTypes -MemoryTypeName Fusion
```

Example will return glpi Memory Types, but what is the most important, Memory Types will be shown exactly as you see in glpi dropdown Memory Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Memory Types from GLPI

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

### -MemoryTypeId
This parameter can take pipline input, either, you can use this function with -MemoryTypeId keyword.
Provide to this param MemoryTypeId from GLPI Memory Types Bookmark

```yaml
Type: String[]
Parameter Sets: MemoryTypeId
Aliases: MTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with MemoryTypeId Parameter.
MemoryTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: MemoryTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MemoryTypeName
This parameter can take pipline input, either, you can use this function with -MemoryTypeId keyword.
Provide to this param Memory Types Name from GLPI Memory Types Bookmark

```yaml
Type: String
Parameter Sets: MemoryTypeName
Aliases: MTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Memory Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Memory Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
