---
title: Get-GlpiToolsDropdownsInterfaceHardDriveTypes
---

## SYNOPSIS
Function is getting Interface Hard Drive Types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes [-All] [<CommonParameters>]
```

### InterfaceHardDriveTypeId
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -InterfaceHardDriveTypeId <String[]> [-Raw] [<CommonParameters>]
```

### InterfaceHardDriveTypeName
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -InterfaceHardDriveTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on InterfaceHardDriveTypeId which you can find in GLPI website
Returns object with property's of Interface Hard Drive Types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -All
```

Example will return all Interface Hard Drive Types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsInterfaceHardDriveTypes
```

Function gets InterfaceHardDriveTypeId from GLPI from Pipline, and return Interface Hard Drive Types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsInterfaceHardDriveTypes
```

Function gets InterfaceHardDriveTypeId from GLPI from Pipline (u can pass many ID's like that), and return Interface Hard Drive Types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -InterfaceHardDriveTypeId 326
```

Function gets InterfaceHardDriveTypeId from GLPI which is provided through -InterfaceHardDriveTypeId after Function type, and return Interface Hard Drive Types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -InterfaceHardDriveTypeId 326, 321
```

Function gets Interface Hard Drive Types Id from GLPI which is provided through -InterfaceHardDriveTypeId keyword after Function type (u can provide many ID's like that), and return Interface Hard Drive Types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsInterfaceHardDriveTypes -InterfaceHardDriveTypeName Fusion
```

Example will return glpi Interface Hard Drive Types, but what is the most important, Interface Hard Drive Types will be shown exactly as you see in glpi dropdown Interface Hard Drive Types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Interface Hard Drive Types from GLPI

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

### -InterfaceHardDriveTypeId
This parameter can take pipline input, either, you can use this function with -InterfaceHardDriveTypeId keyword.
Provide to this param InterfaceHardDriveTypeId from GLPI Interface Hard Drive Types Bookmark

```yaml
Type: String[]
Parameter Sets: InterfaceHardDriveTypeId
Aliases: IHDTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with InterfaceHardDriveTypeId Parameter.
InterfaceHardDriveTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: InterfaceHardDriveTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -InterfaceHardDriveTypeName
This parameter can take pipline input, either, you can use this function with -InterfaceHardDriveTypeId keyword.
Provide to this param Interface Hard Drive Types Name from GLPI Interface Hard Drive Types Bookmark

```yaml
Type: String
Parameter Sets: InterfaceHardDriveTypeName
Aliases: IHDTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Interface Hard Drive Types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Interface Hard Drive Types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
