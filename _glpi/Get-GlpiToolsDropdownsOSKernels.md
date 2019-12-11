---
title: Get-GlpiToolsDropdownsOSKernels
---

## SYNOPSIS
Function is getting OS Kernels informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSKernels [-All] [<CommonParameters>]
```

### OSKernelId
```
Get-GlpiToolsDropdownsOSKernels -OSKernelId <String[]> [-Raw] [<CommonParameters>]
```

### OSKernelName
```
Get-GlpiToolsDropdownsOSKernels -OSKernelName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSKernelId which you can find in GLPI website
Returns object with property's of OS Kernels

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSKernels -All
```

Example will return all OS Kernels from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSKernels
```

Function gets OSKernelId from GLPI from Pipline, and return OS Kernels object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSKernels
```

Function gets OSKernelId from GLPI from Pipline (u can pass many ID's like that), and return OS Kernels object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSKernels -OSKernelId 326
```

Function gets OSKernelId from GLPI which is provided through -OSKernelId after Function type, and return OS Kernels object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSKernels -OSKernelId 326, 321
```

Function gets OS KernelsId from GLPI which is provided through -OSKernelId keyword after Function type (u can provide many ID's like that), and return OS Kernels object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSKernels -OSKernelName Fusion
```

Example will return glpi OS Kernels, but what is the most important, OS Kernels will be shown exactly as you see in glpi dropdown OS Kernels.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all OS Kernels from GLPI

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

### -OSKernelId
This parameter can take pipline input, either, you can use this function with -OSKernelId keyword.
Provide to this param OSKernelId from GLPI OS Kernels Bookmark

```yaml
Type: String[]
Parameter Sets: OSKernelId
Aliases: OSKID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSKernelId Parameter.
OSKernelId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSKernelId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSKernelName
This parameter can take pipline input, either, you can use this function with -OSKernelId keyword.
Provide to this param OS Kernels Name from GLPI OS Kernels Bookmark

```yaml
Type: String
Parameter Sets: OSKernelName
Aliases: OSKN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### OS Kernels ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of OS Kernels from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
