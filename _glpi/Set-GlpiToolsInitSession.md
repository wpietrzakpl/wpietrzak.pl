---
title: Set-GlpiToolsInitSession
---

## SYNOPSIS
Function which init API session.

## SYNTAX

```
Set-GlpiToolsInitSession [<CommonParameters>]
```

## DESCRIPTION
Function gets nesessery information from Config file, then initialize session, and return object with session_token property.

## EXAMPLES

### EXAMPLE 1
```
Set-GlpiToolsInitSession
```

Run command like that and you will initiate session with API GLPI

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None, inside script Function uses Get-GlpiToolsConfig to get data from Config.
## OUTPUTS

### SessionToken parameter
## NOTES
PSP 12/2018

## RELATED LINKS
