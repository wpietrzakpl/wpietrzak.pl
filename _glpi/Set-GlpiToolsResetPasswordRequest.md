---
title: Set-GlpiToolsResetPasswordRequest
---

## SYNOPSIS
This function is to use for send reset request password for specific user.

## SYNTAX

```
Set-GlpiToolsResetPasswordRequest [-Email] <String> [<CommonParameters>]
```

## DESCRIPTION
This function allows to send reset request password for specific user. 
This function works under the following conditions: * GLPI has notifications enabled * the email address of the user belongs to a user account.

## EXAMPLES

### EXAMPLE 1
```
Set-GlpiToolsPasswordReset -Email "user@domain.com"
```

This example will send an email to user which provided email is belongs to.
Email will have reset link inside the mail.

## PARAMETERS

### -Email
Provide here user email.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Email
## OUTPUTS

### Message which says that email will be send, or throw error with explaination.
## NOTES
PSP 03/2019

## RELATED LINKS
