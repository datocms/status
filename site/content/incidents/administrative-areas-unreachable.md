+++
title = "Administrative areas unreachable"
date = 2018-05-31T17:47:24.000Z
severity = "partial-outage"
affectedsystems = [
  "Administrative areas"
]
resolved = true
+++

The server that hosts our administrative area interface is down.

**Update**: We've identified the issue. The Digital Ocean machine that hosts is having some networking/routing issues: we'll keep you posted in real-time. {{< track "2018-05-31T18:00:11+00:00" >}}
**Update**: The machine is reachable and responds to ping if we perform the request from other locations, so this seems like a localized issue. We're currently working on duplicating the machine. {{< track "2018-05-31T18:10:11+00:00" >}}
**Update**: The duplicate of the machine is almost ready, we should be up and running in approx 15 minutes. {{< track "2018-05-31T18:28:11+00:00" >}}
**Update**: The duplicate of the machine is online. Everything should be working, but we're double checking everything. {{< track "2018-05-31T18:33:11+00:00" >}}
**Update**: Digital Ocean has just implemented a fix. More details here: https://status.digitalocean.com/incidents/fq8nt7bfrclx We'll switch back to our original instance once everything is resolved. {{< track "2018-05-31T18:49:11+00:00" >}}



