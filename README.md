# batch-Notes
Personal notebook of batch commands

## Parameters
### System Parameters
`%SystemRoot%` C:\Windwos(%windir%) \
`%ProgramFiles%` C:\Program Files \
`%USERPROFILE%` C:\Documents and Settings\Administrator \
`%APPDATA%` C:\Documents and Settings\Administrator\Application Data \
`%TEMP%` C:\DOCUME~1\ADMINI~1\LOCALS~1\Temp \
`%OS%` Windows_NT \
`%HOMEDRIVE%` C: \
`setlocal enabledelayedexpansion` any env variable changes are lost at the end of a batch script \
`FOR /F "usebackq delims==" %%i IN(set) DO `

### Parameters pass to the batch file
%[1-9] \
`%0` batch itself \
`%1` first parameter \

## Commands
#### %~dp0 
d: Drive \
p: path

`cd %~dp0` \
change directory into current batch file path \

`cd %~dp0bin` \
change directory into bin of current batch file path


`%cd%` \
current directory \

`taskkill /f /im notepad.exe` \
terminate process notepad.exe \


#### ECHO
`ECHO [{on|off}] [message]` \
`echo off` \
`echo Windows Registry Editor Version 5.00 > C:\setupreg.reg` create file setupreg.reg \
`echo "SourcePath"="D:\\Win2003\\" >> C:\setupreg.reg` add to file \

#### GOTO
`goto label` 

#### CALL
`call [[Drive:][Path]FileName[BatchParameters]][:label [aruments]] \
call another batch file, get back to parent job from  

#### START
call another exec or DOS commands \
`START /MIN /HIGH /SEPARATE /REALTIME /WAIT` 

#### IF
`IF [NOT] [condition]` \
`IF [NOT] exist [path]` \
`IF [NOT] ERRORLEVEL <number>` \
`IF ELSE` \ 


#### Comparison
`EQU` "==" \
`NEQ` "!=" \
`LSS` "<" \
`LEQ` "<=" \
`GTR` ">" \
`GEQ` ">=" \

#### CHOICE

#### FOR
|||
|---|---|
|FOR {%variable \| %%variable} IN (set) DO COMMAND [COMMAND-PARAMETERS]||


