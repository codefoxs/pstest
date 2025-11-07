# pstest
A modified version for Stata command pstest.

# PSM

```Stata
psmatch2 Treat X1 X2 X3, out(Y) n(1) cal(0.01) logit ate common ties

run "mypstest.do" // download from my repository
pstest X1 X2 X3, both graph

psm2dta
save "PSM table.dta", replace
```

# ebalance
```Stata
ebalance Treat X1 X2 X3 , tar(1)
run "mypstest.do" // download from my repository

eb2dta
save "Ebalance table.dta", replace
```
