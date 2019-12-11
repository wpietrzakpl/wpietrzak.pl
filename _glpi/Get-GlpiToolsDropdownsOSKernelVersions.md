---
title: Get-GlpiToolsDropdownsOSKernelVersions
---

## SYNOPSIS
Function is getting OS Kernel Versions informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsOSKernelVersions [-All] [<CommonParameters>]
```

### OSKernelVersionId
```
Get-GlpiToolsDropdownsOSKernelVersions -OSKernelVersionId <String[]> [-Raw] [<CommonParameters>]
```

### OSKernelVersionName
```
Get-GlpiToolsDropdownsOSKernelVersions -OSKernelVersionName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on OSKernelVersionId which you can find in GLPI website
Returns object with property's of OS Kernel Versions

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsOSKernelVersions -All
```

Example will return all OS Kernel Versions from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsOSKernelVersions
```

Function gets OSKernelVersionId from GLPI from Pipline, and return OS Kernel Versions object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsOSKernelVersions
```

Function gets OSKernelVersionId from GLPI from Pipline (u can pass many ID's like that), and return OS Kernel Versions object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsOSKernelVersions -OSKernelVersionId 326
```

Function gets OSKernelVersionId from GLPI which is provided through -OSKernelVersionId after Function type, and return OS Kernel Versions object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsOSKernelVersions -OSKernelVersionId 326, 321
```

Function gets OS Kernel VersionsId from GLPI which is provided through -OSKernelVersionId keyword after Function type (u can provide many ID's like that), and return OS Kernel Versions object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsOSKernelVersions -OSKernelVersionName Fusion
```

Example will return glpi OS Kernel Versions, but what is the most important, OS Kernel Versions will be shown exactly as you see in glpi dropdown OS Kernel Versions.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all OS Kernel Versions from GLPI

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

### -OSKernelVersionId
This parameter can take pipline input, either, you can use this function with -OSKernelVersionId keyword.
Provide to this param OSKernelVersionId from GLPI OS Kernel Versions Bookmark

```yaml
Type: String[]
Parameter Sets: OSKernelVersionId
Aliases: OSKVID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with OSKernelVersionId Parameter.
OSKernelVersionId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: OSKernelVersionId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OSKernelVersionName
This parameter can take pipline input, either, you can use this function with -OSKernelVersionId keyword.
Provide to this param OS Kernel Versions Name from GLPI OS Kernel Versions Bookmark

```yaml
Type: String
Parameter Sets: OSKernelVersionName
Aliases: OSKVN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### OS Kernel Versions ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of OS Kernel Versions from GLPI
## NOTES
PSP 08/2019

## RELATED LINKS
