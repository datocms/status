+++
title = "Slow responses and intermittent 503 error codes"
date = 2018-11-14T13:09:10.000Z
severity = "degraded-performance"
affectedsystems = [
  "API"
]
resolved = true
+++
We're receiving feedback of slow responses and intermittent 503 error codes on our Content Management API, we've doubled up our server resources and investigating in the meantime

**Update**: The problem was due to some memory corruption issues on the server caused by some C extensions. We tracked down the issue and shipped a fix. We'll continue monitoring the situation. {{< track "2018-11-14T17:09:10.000Z" >}}
