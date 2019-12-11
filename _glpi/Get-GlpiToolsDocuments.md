---
title: Get-GlpiToolsDocuments
---

## SYNOPSIS
Function is getting Document informations from GLPI

## SYNTAX

### DocumentId (Default)
```
Get-GlpiToolsDocuments [-DocumentId] <Int32[]> [<CommonParameters>]
```

### All
```
Get-GlpiToolsDocuments [-All] [<CommonParameters>]
```

### RawDocument
```
Get-GlpiToolsDocuments [[-DocumentId] <Int32[]>] [-RawDocument] [<CommonParameters>]
```

### Raw
```
Get-GlpiToolsDocuments [[-DocumentId] <Int32[]>] [-Raw] [<CommonParameters>]
```

## DESCRIPTION
Function is based on DocumentID which you can find in GLPI website
Returns object with property's of document.

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDocuments -All
```

Example will show all documents from Document GLPI Bookmark.

### EXAMPLE 2
```
Get-GlpiToolsDocuments -ComputerId 2
```

Example will return object of document which id is 2.
Example will convert values to human readable.

### EXAMPLE 3
```
Get-GlpiToolsDocuments -ComputerId 2 -Raw
```

Example will return object of document which id is 2.
Example will not convert values to human readable.

### EXAMPLE 4
```
Get-GlpiToolsDocuments -ComputerId 2 -RawDocument
```

Example will return content which document has inside the file.

## PARAMETERS

### -All
This parameter will return all documents from GLPI

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

### -DocumentId
This parameter can take pipline input, either, you can use this function with -DocumentId keyword.
Provide to this param Document ID from GLPI Documents Bookmark

```yaml
Type: Int32[]
Parameter Sets: DocumentId
Aliases: DocID

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: Int32[]
Parameter Sets: RawDocument, Raw
Aliases: DocID

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DocumentId Parameter.
DocumentId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: Raw
Aliases:

Required: False
Position: 2
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RawDocument
Parameter which you can use with DocumentId Parameter.
This parameter get document and return what document has inside.

```yaml
Type: SwitchParameter
Parameter Sets: RawDocument
Aliases:

Required: False
Position: 2
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Document ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of document's from GLPI
## NOTES
PSP 05/2019

## RELATED LINKS
