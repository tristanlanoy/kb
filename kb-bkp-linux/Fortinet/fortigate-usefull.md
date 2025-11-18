# Fortigate usefull commands

## Auto revert

```fortios
config system global
    set cfg-save revert
    set cfg-revert-timeout 600 <- The default is 600s of admin session being idle.
end
```

Equivalent to Cisco write mem :  
`execute cfg save`

Otherwise auto rollback at the end of the timeout.  
