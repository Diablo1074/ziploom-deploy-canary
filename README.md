# ziploom-deploy-canary

A deliberately trivial **public** static site used to prove the ZipLoom deploy
pipeline end to end.

Why it looks like nothing: it is supposed to. No framework, no build step, no
dependencies, no environment variables, no database. If a deploy of this repo
fails, the failure is in the pipeline — not in the customer's app. That is the
entire point.

`index.html` contains the marker `canary-v1`, which the health check and any
post-deploy verification can look for in the response body.
