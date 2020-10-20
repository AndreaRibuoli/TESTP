# TESTP
Test PASERIE internals

```
PASERIE/INSTALL GIT_USER(AndreaRibuoli) PACKAGEN(TESTP)        
```

## tuning behaviour

PASERIE/INSTALL transfers an **installation mode** value to the **BUILD** program (compiled in QTEMP).
This value can be tested to differentiate behaviour.
It is called `DEVOPT` and is defined as a `CHAR(1)`.

When **Y** che convention is that the source files are to be copied from QTEMP to the target library.
The save BUILD program (CLLE) will be compiled and will behave differently assuming the CHAR(1) argument 
is omitted. Missing argument default to **L** value for *Local build*.

When **N** (the default value PASERIE/INSTALL passes to BUILD) the build is supposed to execute in QTEMP 
without saving source files.
