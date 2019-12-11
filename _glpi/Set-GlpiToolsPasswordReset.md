---
title: Set-GlpiToolsPasswordReset
---

## SYNOPSIS
This function is to use for reset password for specific user.

## SYNTAX

```
Set-GlpiToolsPasswordReset [-Email] <String> [-Password] <String> [[-PasswordForgetToken] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
This function allows to reset password for specific user. 
This function works under the following conditions: * GLPI has notifications enabled * the email address of the user belongs to a user account.

## EXAMPLES

### EXAMPLE 1
```
Set-GlpiToolsPasswordReset -Email "user@domain.com" -Password "NewPassword" -PasswordForgetToken "b0a4cfe81448299ebed57442f4f21929c80ebee5"
```

This example will send an email to user which provided email is belongs to, and reset his password for defined value.
Example will renew user_token.

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

### -Password
Provide here new password for user.

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

### -PasswordForgetToken
Provide here old user user_token, for the new one.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Email, Password, User_Token
## OUTPUTS

### Message which says that email will be send, or throw error with explaination.
## NOTES
PSP 03/2019

## RELATED LINKS
