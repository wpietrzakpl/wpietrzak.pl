---
title: Get-GlpiToolsSoftware
---

## SYNOPSIS
Function is getting Software informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsSoftware [-All] [<CommonParameters>]
```

### SoftwareId
```
Get-GlpiToolsSoftware -SoftwareId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### SoftwareName
```
Get-GlpiToolsSoftware -SoftwareName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on SoftwareID which you can find in GLPI website
Returns object with property's of Software

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsSoftware
```

Function gets SoftwareId from GLPI from Pipline, and return Software object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsSoftware
```

Function gets SoftwareId from GLPI from Pipline (u can pass many ID's like that), and return Software object

### EXAMPLE 3
```
Get-GlpiToolsSoftware -SoftwareId 326
```

Function gets SoftwareId from GLPI which is provided through -SoftwareId after Function type, and return Software object

### EXAMPLE 4
```
Get-GlpiToolsSoftware -SoftwareId 326, 321
```

Function gets SoftwareId from GLPI which is provided through -SoftwareId keyword after Function type (u can provide many ID's like that), and return Software object

## PARAMETERS

### -All
This parameter will return all Softwares from GLPI

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

### -SoftwareId
This parameter can take pipline input, either, you can use this function with -SoftwareId keyword.
Provide to this param Software ID from GLPI Softwares Bookmark

```yaml
Type: String[]
Parameter Sets: SoftwareId
Aliases: SID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with SoftwareId Parameter.
SoftwareId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: SoftwareId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with SoftwareId Parameter. 
If you want to get additional parameter of Software object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: SoftwareId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SoftwareName
This parameter can take pipline input, either, you can use this function with -SoftwareName keyword.
Provide to this param Software Name from GLPI Softwares Bookmark

```yaml
Type: String
Parameter Sets: SoftwareName
Aliases: SN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with SoftwareName Parameter.
If you want Search for Software name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: SoftwareName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Software ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of software from GLPI
## NOTES
PSP 04/2019

## RELATED LINKS
