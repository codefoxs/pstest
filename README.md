# pstest
A modified version for Stata command pstest.

# Quick use

```Stata
psmatch2 Treat X1 X2 X3, out(Y) n(1) cal(0.01) logit ate common ties

run "mypstest.do" // download from my repository
pstest X1 X2 X3, both graph

preserve
psm2dta r(result_matrix)
save "PSM table.dta", replace
restore
```
