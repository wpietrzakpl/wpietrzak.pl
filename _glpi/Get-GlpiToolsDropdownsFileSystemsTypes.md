---
title: Get-GlpiToolsDropdownsFileSystemsTypes
---

## SYNOPSIS
Function is getting File Systems Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsFileSystemsTypes [-All] [<CommonParameters>]
```

### FileSystemTypeId
```
Get-GlpiToolsDropdownsFileSystemsTypes -FileSystemTypeId <String[]> [-Raw] [<CommonParameters>]
```

### FileSystemTypeName
```
Get-GlpiToolsDropdownsFileSystemsTypes -FileSystemTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on FileSystemTypeId which you can find in GLPI website
Returns object with property's of File Systems Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsFileSystemsTypes -All
```

Example will return all File Systems Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsFileSystemsTypes
```

Function gets FileSystemTypeId from GLPI from Pipline, and return File Systems Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsFileSystemsTypes
```

Function gets FileSystemTypeId from GLPI from Pipline (u can pass many ID's like that), and return File Systems Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsFileSystemsTypes -FileSystemTypeId 326
```

Function gets FileSystemTypeId from GLPI which is provided through -FileSystemTypeId after Function type, and return File Systems Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsFileSystemsTypes -FileSystemTypeId 326, 321
```

Function gets File Systems Types Id from GLPI which is provided through -FileSystemTypeId keyword after Function type (u can provide many ID's like that), and return File Systems Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsFileSystemsTypes -FileSystemTypeName Fusion
```

Example will return glpi File Systems Types, but what is the most important, File Systems Types will be shown exactly as you see in glpi dropdown File Systems Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all File Systems Types from GLPI

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

### -FileSystemTypeId
This parameter can take pipline input, either, you can use this function with -FileSystemTypeId keyword.
Provide to this param FileSystemTypeId from GLPI File Systems Types Bookmark

```yaml
Type: String[]
Parameter Sets: FileSystemTypeId
Aliases: FSTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with FileSystemTypeId Parameter.
FileSystemTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: FileSystemTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileSystemTypeName
This parameter can take pipline input, either, you can use this function with -FileSystemTypeId keyword.
Provide to this param File Systems Types Name from GLPI File Systems Types Bookmark

```yaml
Type: String
Parameter Sets: FileSystemTypeName
Aliases: FSTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### File Systems Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of File Systems Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
