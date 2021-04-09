---
type: decision
acronym: browser
title: >
    Google Chrome and Firefox are the optimized browsers
decision_type: must
belongs_to: devops
status: _3_sig_agreed
responsible: JSP
deadline: 2021-04-16
implemented: partially
history:
    v1:
        date: 2021-04-16
        comment: created initially
---

## Why is there need for such a decision?

Nowadays it is important to decide which browser is taking as the "truth". 
There are many browsers out there, although not all are known.
The best known are Google Chrome, Firefox, Internet Explorer (Edge) and Safari (possibly also Opera).

## Additional sources for better understanding the background

[Browser Market Share Worldwide Mar 2021](https://gs.statcounter.com/browser-market-share#monthly-202103-202103-bar).

[Angular Browser Support](https://angular.io/guide/browser-support).

[Safari Windows Support](https://support.apple.com/en-us/HT204416).


## How is this decision evaluated?

It was made a quick research about the supported Browser from Angular and which browser are often used.
 
## Resolution Details

Since the current version of Safari can only be used on MAC, it is no longer considered.
Of the first three, only Google Chrome and Firefox remain. 
Not to forget that Edge is based on Google Chrome.
