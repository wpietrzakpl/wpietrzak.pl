---
title: Get-GlpiToolsDropdownsDocumentTypes
---

## SYNOPSIS
Function is getting Document types informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDocumentTypes [-All] [<CommonParameters>]
```

### DocumentTypeId
```
Get-GlpiToolsDropdownsDocumentTypes -DocumentTypeId <String[]> [-Raw] [<CommonParameters>]
```

### DocumentTypeName
```
Get-GlpiToolsDropdownsDocumentTypes -DocumentTypeName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DocumentTypeId which you can find in GLPI website
Returns object with property's of Document types

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDocumentTypes -All
```

Example will return all Document types from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDocumentTypes
```

Function gets DocumentTypeId from GLPI from pipeline, and return Document types object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDocumentTypes
```

Function gets DocumentTypeId from GLPI from pipeline (u can pass many ID's like that), and return Document types object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDocumentTypes -DocumentTypeId 326
```

Function gets DocumentTypeId from GLPI which is provided through -DocumentTypeId after Function type, and return Document types object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDocumentTypes -DocumentTypeId 326, 321
```

Function gets Document types Id from GLPI which is provided through -DocumentTypeId keyword after Function type (u can provide many ID's like that), and return Document types object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDocumentTypes -DocumentTypeName Fusion
```

Example will return glpi Document types, but what is the most important, Document types will be shown exactly as you see in glpi dropdown Document types.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Document types from GLPI

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

### -DocumentTypeId
This parameter can take pipeline input, either, you can use this function with -DocumentTypeId keyword.
Provide to this param DocumentTypeId from GLPI Document types Bookmark

```yaml
Type: String[]
Parameter Sets: DocumentTypeId
Aliases: DTID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DocumentTypeId Parameter.
DocumentTypeId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DocumentTypeId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocumentTypeName
This parameter can take pipeline input, either, you can use this function with -DocumentTypeId keyword.
Provide to this param Document types Name from GLPI Document types Bookmark

```yaml
Type: String
Parameter Sets: DocumentTypeName
Aliases: DTN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Document types ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Document types from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
