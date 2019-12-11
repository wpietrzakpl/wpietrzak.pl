---
title: Get-GlpiToolsRssFeeds
---

## SYNOPSIS
Function is getting RSS feeds informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsRssFeeds [-All] [<CommonParameters>]
```

### RssfeedId
```
Get-GlpiToolsRssFeeds -RssfeedId <String[]> [-Raw] [<CommonParameters>]
```

### RssfeedName
```
Get-GlpiToolsRssFeeds -RssfeedName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on RssfeedId which you can find in GLPI website
Returns object with property's of RSS feeds

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsRssFeeds -All
```

Example will return all RSS feeds from Glpi

### EXAMPLE 2
```
326 | Get-GlpiToolsRssFeeds
```

Function gets RssfeedId from GLPI from Pipline, and return RSS feeds object

### EXAMPLE 3
```
326, 321 | Get-GlpiToolsRssFeeds
```

Function gets RssfeedId from GLPI from Pipline (u can pass many ID's like that), and return RSS feeds object

### EXAMPLE 4
```
Get-GlpiToolsRssFeeds -RssfeedId 326
```

Function gets RssfeedId from GLPI which is provided through -RssfeedId after Function type, and return RSS feeds object

### EXAMPLE 5
```
Get-GlpiToolsRssFeeds -RssfeedId 326, 321
```

Function gets RSS feeds Id from GLPI which is provided through -RssfeedId keyword after Function type (u can provide many ID's like that), and return RSS feeds object

### EXAMPLE 6
```
Get-GlpiToolsRssFeeds -RssfeedName Fusion
```

Example will return glpi RSS feeds, but what is the most important, RSS feeds will be shown exactly as you see in glpi dropdown RSS feeds.
If you want to add parameter, you have to modify "default items to show".
This is the "key/tool" icon near search.

## PARAMETERS

### -All
This parameter will return all RSS feeds from GLPI

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

### -RssfeedId
This parameter can take pipline input, either, you can use this function with -RssfeedId keyword.
Provide to this param RssfeedId from GLPI RSS feeds Bookmark

```yaml
Type: String[]
Parameter Sets: RssfeedId
Aliases: RFID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with RssfeedId Parameter.
RssfeedId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: RssfeedId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RssfeedName
This parameter can take pipline input, either, you can use this function with -RssfeedId keyword.
Provide to this param RSS feeds Name from GLPI RSS feeds Bookmark

```yaml
Type: String
Parameter Sets: RssfeedName
Aliases: RFN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### RSS feeds ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of RSS feeds from GLPI
## NOTES
PSP 11/2019

## RELATED LINKS
