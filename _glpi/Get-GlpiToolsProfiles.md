---
title: Get-GlpiToolsProfiles
---

## SYNOPSIS
Function is getting Profile informations from GLPI

## SYNTAX

### All
```
Get-GlpiToolsProfiles [-All] [<CommonParameters>]
```

### ProfileId
```
Get-GlpiToolsProfiles -ProfileId <String[]> [-Raw] [<CommonParameters>]
```

### ProfileName
```
Get-GlpiToolsProfiles -ProfileName <String> [<CommonParameters>]
```

## DESCRIPTION
Function is based on ProfileID which you can find in GLPI website
Returns object with property's of Profile

## EXAMPLES

### EXAMPLE 1
```
Get-GlpiToolsProfiles -All
```

Example will show all profiles.

### EXAMPLE 2
```
Get-GlpiToolsProfiles -ProfileName Admin
```

Example will return every profile which contains Admin keyword

## PARAMETERS

### -All
This parameter will return all Profiles from GLPI

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

### -ProfileId
This parameter can take pipline input, either, you can use this function with -ProfileId keyword.
Provide to this param Profile ID from GLPI Profile Bookmark

```yaml
Type: String[]
Parameter Sets: ProfileId
Aliases: PID

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Raw
Parameter which you can use with ProfileId Parameter.
ProfileId has converted parameters from default, parameter Raw allows not convert this parameters.

```yaml
Type: SwitchParameter
Parameter Sets: ProfileId
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProfileName
This parameter can take pipline input, either, you can use this function with -ProfileName keyword.
Provide to this param Profile Name from GLPI Profiles Bookmark

```yaml
Type: String
Parameter Sets: ProfileName
Aliases: PN

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Profile ID which you can find in GLPI, or use this Function to convert ID returned from other Functions
## OUTPUTS

### Function returns PSCustomObject with property's of Profiles from GLPI
## NOTES
PSP 04/2019

## RELATED LINKS
