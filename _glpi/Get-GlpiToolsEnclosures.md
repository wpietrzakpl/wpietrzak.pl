---
title: Get-GlpiToolsEnclosures
---

## SYNOPSIS
Function is getting Enclosure informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsEnclosures [-All] [<CommonParameters>]
```

### EnclosureId
```
Get-GlpiToolsEnclosures -EnclosureId <String[]> [-Raw] [-Parameter <String>] [<CommonParameters>]
```

### EnclosureName
```
Get-GlpiToolsEnclosures -EnclosureName <String> [-SearchInTrash <String>] [<CommonParameters>]
```

## DESCRIPTION
Function is based on EnclosureID which you can find in GLPI website
Returns object with property's of Enclosure

## EXAMPLES

### EXAMPLE 1
```
326 | Get-GlpiToolsEnclosures
```

Function gets EnclosureID from GLPI from Pipline, and return Enclosure object

### EXAMPLE 2
```
326, 321 | Get-GlpiToolsEnclosures
```

Function gets EnclosureID from GLPI from Pipline (u can pass many ID's like that), and return Enclosure object

### EXAMPLE 3
```
Get-GlpiToolsEnclosures -EnclosureId 326
```

Function gets EnclosureID from GLPI which is provided through -EnclosureId after Function type, and return Enclosure object

### EXAMPLE 4
```
Get-GlpiToolsEnclosures -EnclosureId 326, 321
```

Function gets EnclosureID from GLPI which is provided through -EnclosureId keyword after Function type (u can provide many ID's like that), and return Enclosure object

### EXAMPLE 5
```
Get-GlpiToolsEnclosures -EnclosureId 234 -Raw
```

Example will show Enclosure with id 234, but without any parameter converted

### EXAMPLE 6
```
234 | Get-GlpiToolsEnclosures -Raw
```

Example will show Enclosure with id 234, but without any parameter converted

### EXAMPLE 7
```
Get-GlpiToolsEnclosures -EnclosureName glpi
```

Example will return glpi Enclosure, but what is the most important, Enclosure will be shown exacly as you see in glpi Enclosures tab.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

### EXAMPLE 8
```
Get-GlpiToolsEnclosures -EnclosureName glpi -SearchInTrash Yes
```

Example will return glpi Enclosure, but from trash

## PARAMETERS

### -All
This parameter will return all Enclosures from GLPI

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

### -EnclosureId
This parameter can take pipline input, either, you can use this function with -EnclosureId keyword.
Provide to this param Enclosure ID from GLPI Enclosures Bookmark

```yaml
Type: String[]
Parameter Sets: EnclosureId
Aliases: EID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with EnclosureId Parameter.
EnclosureId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: EnclosureId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnclosureName
Provide to this param Enclosure Name from GLPI Enclosures Bookmark

```yaml
Type: String
Parameter Sets: EnclosureName
Aliases: EN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchInTrash
Parameter which you can use with EnclosureName Parameter.
If you want Search for Enclosure name in trash, that parameter allow you to do it.

```yaml
Type: String
Parameter Sets: EnclosureName
Aliases: SIT

Required: False
Position: Named
Default value: No
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
Parameter which you can use with EnclosureId Parameter. 
If you want to get additional parameter of Enclosure object like, disks, or logs, use this parameter.

```yaml
Type: String
Parameter Sets: EnclosureId
Aliases: Param

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Enclosure ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Enclosures from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
