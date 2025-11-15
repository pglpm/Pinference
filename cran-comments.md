## R CMD check results

0 errors | 0 warnings | 1 note

* The URL https://encyclopediaofmath.org/wiki/Sequent_calculus (in vignette) is down, but just momentarily.


## revdepcheck results

No reverse dependencies.


## Minor update

Addresses possible unintended misuse of logical notation within inferP(), with operator-precedence quirks that the user may be unaware of:

* Improved documentation about the two available kinds of logical notation.

* inferP() now issues a warning if `!` operator is used in combination with `*`, `+`, `>` since this may lead to unintended operator precedence (see point above).

* Function `ifthen()` can now be used within logical notation instead of `>` (again to avoid operator-precedence quirks).
