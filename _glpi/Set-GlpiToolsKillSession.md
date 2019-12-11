---
title: Set-GlpiToolsKillSession
---

## SYNOPSIS
Function which kill API session.

## SYNTAX

```
Set-GlpiToolsKillSession [[-SessionToken] <String>] [<CommonParameters>]
```

## DESCRIPTION
Function gets nesessery information from Config file, and Function Set-GlpiToolsInitSession, then kill session.

## EXAMPLES

### EXAMPLE 1
```
$SessionToken | Set-GlpiToolsKillSession
```

Run command like that and you will kill session with API GLPI

### EXAMPLE 2
```
Set-GlpiToolsKillSession -SessionToken $SessionToken
```

Run command like that and you will kill session with API GLPI

## PARAMETERS

### -SessionToken
This parameter have to be passed from Set-GlpiToolsInitSession

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### SessionToken from Set-GlpiToolsInitSession
## OUTPUTS

### None
## NOTES
PSP 12/2018

## RELATED LINKS
