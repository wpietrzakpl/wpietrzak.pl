---
title: Get-GlpiToolsDropdownsVirtualizationSystems
---

## SYNOPSIS
Function is getting Virtualization Systems informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsVirtualizationSystems [-All] [<CommonParameters>]
```

### VirtualizationSystemId
```
Get-GlpiToolsDropdownsVirtualizationSystems -VirtualizationSystemId <String[]> [-Raw] [<CommonParameters>]
```

### VirtualizationSystemName
```
Get-GlpiToolsDropdownsVirtualizationSystems -VirtualizationSystemName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on VirtualizationSystemId which you can find in GLPI website
Returns object with property's of Virtualization Systems

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsVirtualizationSystems -All
```

Example will return all Virtualization Systems from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsVirtualizationSystems
```

Function gets VirtualizationSystemId from GLPI from pipeline, and return Virtualization Systems object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsVirtualizationSystems
```

Function gets VirtualizationSystemId from GLPI from pipeline (u can pass many ID's like that), and return Virtualization Systems object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsVirtualizationSystems -VirtualizationSystemId 326
```

Function gets VirtualizationSystemId from GLPI which is provided through -VirtualizationSystemId after Function type, and return Virtualization Systems object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsVirtualizationSystems -VirtualizationSystemId 326, 321
```

Function gets Virtualization Systems Id from GLPI which is provided through -VirtualizationSystemId keyword after Function type (u can provide many ID's like that), and return Virtualization Systems object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsVirtualizationSystems -VirtualizationSystemName Fusion
```

Example will return glpi Virtualization Systems, but what is the most important, Virtualization Systems will be shown exactly as you see in glpi dropdown Virtualization Systems.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Virtualization Systems from GLPI

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

### -VirtualizationSystemId
This parameter can take pipeline input, either, you can use this function with -VirtualizationSystemId keyword.
Provide to this param VirtualizationSystemId from GLPI Virtualization Systems Bookmark

```yaml
Type: String[]
Parameter Sets: VirtualizationSystemId
Aliases: VSID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with VirtualizationSystemId Parameter.
VirtualizationSystemId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: VirtualizationSystemId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -VirtualizationSystemName
This parameter can take pipeline input, either, you can use this function with -VirtualizationSystemId keyword.
Provide to this param Virtualization Systems Name from GLPI Virtualization Systems Bookmark

```yaml
Type: String
Parameter Sets: VirtualizationSystemName
Aliases: VSN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Virtualization Systems ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Virtualization Systems from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
