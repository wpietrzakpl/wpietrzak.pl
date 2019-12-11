---
title: Get-GlpiToolsDropdownsDocumentHeadings
---

## SYNOPSIS
Function is getting Document headings informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsDropdownsDocumentHeadings [-All] [<CommonParameters>]
```

### DocumentHeadingId
```
Get-GlpiToolsDropdownsDocumentHeadings -DocumentHeadingId <String[]> [-Raw] [<CommonParameters>]
```

### DocumentHeadingName
```
Get-GlpiToolsDropdownsDocumentHeadings -DocumentHeadingName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on DocumentHeadingId which you can find in GLPI website
Returns object with property's of Document headings

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsDropdownsDocumentHeadings -All
```

Example will return all Document headings from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsDropdownsDocumentHeadings
```

Function gets DocumentHeadingId from GLPI from pipeline, and return Document headings object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsDropdownsDocumentHeadings
```

Function gets DocumentHeadingId from GLPI from pipeline (u can pass many ID's like that), and return Document headings object

### EXAMPLE 4
```
Get-GlpiToolsDropdownsDocumentHeadings -DocumentHeadingId 326
```

Function gets DocumentHeadingId from GLPI which is provided through -DocumentHeadingId after Function type, and return Document headings object

### EXAMPLE 5
```
Get-GlpiToolsDropdownsDocumentHeadings -DocumentHeadingId 326, 321
```

Function gets Document headings Id from GLPI which is provided through -DocumentHeadingId keyword after Function type (u can provide many ID's like that), and return Document headings object

### EXAMPLE 6
```
Get-GlpiToolsDropdownsDocumentHeadings -DocumentHeadingName Fusion
```

Example will return glpi Document headings, but what is the most important, Document headings will be shown exactly as you see in glpi dropdown Document headings.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all Document headings from GLPI

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

### -DocumentHeadingId
This parameter can take pipeline input, either, you can use this function with -DocumentHeadingId keyword.
Provide to this param DocumentHeadingId from GLPI Document headings Bookmark

```yaml
Type: String[]
Parameter Sets: DocumentHeadingId
Aliases: DHID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with DocumentHeadingId Parameter.
DocumentHeadingId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: DocumentHeadingId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocumentHeadingName
This parameter can take pipeline input, either, you can use this function with -DocumentHeadingId keyword.
Provide to this param Document headings Name from GLPI Document headings Bookmark

```yaml
Type: String
Parameter Sets: DocumentHeadingName
Aliases: DHN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Document headings ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Document headings from GLPI
## NOTES
PSP 09/2019

## RELATED LINKS
