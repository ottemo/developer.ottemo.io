+++
title = "Overview"
weight  = 1
creatordisplayname = "James  Vastbinder"
creatoremail = "james@ottemo.io"
lastmodifierdisplayname = "James Vastbinder"
lastmodifieremail = "james@ottemo.io"
date =  "2017-01-12"
+++

Ottemo is an ecommerce engine created as a modular system written in the Golang programming
language. The platform provides merchants with the high performance they need without
sacrificing architectural capabilities developers need.  Ottemo is intended to be customized
and extended at the component level to suite each retailer’s specific needs.

<img src="/images/OttemoStackDiagram.svg" alt="Overview of Ottemo" height=540px>

Currently there are 3 services which make up the Ottemo stack:

1. **foundation** - an elegant monolith written in Golang
2. **store** - a web store written in any frontend technology supporting REST
3. **dashboard** - an administration panel for merchants

It is not limited to only these applications and may be customized to provide a drop-in backend
for native mobile applications for similar purposes, and of course you can provide your own
subsystem to feed the Foundation service with requests. While we have chose to expose a
REST api, an interface for websockets or GRPC may be quickly developed.

Both Store and Dashboard are optional systems and can be located on the same host with
Foundation, as well as stand alone. Whereas Store and Dashboard subsystems are both based
on the AngularJS framework, this offloads process execution to the client’s side (client’s device), which
significantly reduces the load to the server host(s) allowing extremely efficient use of server resources,
increases throughput and increases the effective performance of the experience.

Ottemo supports the following databases:

1. Sqlite
2. Mongodb
3. Mysql (or any mysql variant)

The target database is configured at compile time to keep the binary as small as possible.
The schema is created the first time Foundation is started if one does not exist. There
are also several starter databases which may be downloaded which have been populated
with sample data to jumpstart development efforts.
