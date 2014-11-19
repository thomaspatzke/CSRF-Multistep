CSRF-Multistep
==============

Framework for building multistep CSRF Proof of Concepts. I use this in web application audits to demonstrate CSRF attacks on workflows that require multiple requests to complete.

Use as follows:

1. Put the start URL in the 'frm.location =' statement in run() or add this as form (see below).

2. Add forms for each needed request in HTML body with form target set to frm. CSRF PoCs from  Burp work well here.

3. Replace next() to load() in iframe onload handler if you need some delay between requests, set needed delay in run.

4. Replace run() with next() in button onclick handler, if first step is requested by form submit.
