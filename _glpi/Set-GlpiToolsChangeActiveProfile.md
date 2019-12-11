---
title: Set-GlpiToolsChangeActiveProfile
---

## SYNOPSIS
Function Change active profile to the profiles_id one.

## SYNTAX

```
Set-GlpiToolsChangeActiveProfile -ProfilesId <Int32> [<CommonParameters>]
```

## DESCRIPTION
Function Change active profile to the profiles_id one.
See Get-GlpiToolsMyProfiles function for possible profiles.

## EXAMPLES

### EXAMPLE 1
```
Set-GlpiToolsChangeActiveProfile -ProfileId 4
```

Example will change active profile on profile with id number 4.

### EXAMPLE 2
```
4 | Set-GlpiToolsChangeActiveProfile
```

Example will change active profile on profile with id number 4.

## PARAMETERS

### -ProfilesId
Parameter which indicate on profile that you will change on.
Provide here an id of this profile.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: PID

Required: True
Position: Named
Default value: 0
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Integer value
## OUTPUTS

### None, or Error if you provide id that not exist.
## NOTES
PSP 04/2019

## RELATED LINKS
