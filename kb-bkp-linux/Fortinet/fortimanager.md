# Fortimanager cheatsheet

## Export objects

` execute fmpolicy print-adom-object <adom_name> ?????? all `

Then use a script to import it in the right ADOM.

## Diganose Auto-Link issues

```fortios
diag debug application securityconsole 255

diag debug service cdb 255

diag debug service cmdb 255

diag debug service dvmcmd 255

diag debug service dvmdb 255

diag debug application dmworker 255

diag debug enable ```
