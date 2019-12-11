---
title: Set-GlpiToolsConfig
---

## SYNOPSIS
Set GLPI Configuration File.

## SYNTAX

```
Set-GlpiToolsConfig [-AppToken] <String> [-UserToken] <String> [-PathToGlpi] <String> [<CommonParameters>]
```

## DESCRIPTION
This function preparing config file for GLPI API.

## EXAMPLES

### EXAMPLE 1
```
Set-GlpiToolsConfig -AppToken 'dsahu2uh2uh32gt43tf434t' -UserToken 'sdasg3123hg3t1ftf21t3' -PathToGlpi 'http://pathtoglpi/glpi'
```

This example show how to set GLPI config file

## PARAMETERS

### -AppToken
Application Token, you can find Token in API Settings at your GLPI website.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserToken
User Token, you can find inside user account settings.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PathToGlpi
Path To GLPI, you can find the path in API Settings at your GLPI website.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None, you cannot pipe objects to Set-GlpiToolsConfig
## OUTPUTS

### None
## NOTES
PSP 12/2018

## RELATED LINKS
