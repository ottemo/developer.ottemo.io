+++
type="HomePage"
creatordisplayname = "James  Vastbinder"
creatoremail = "james@ottemo.io"
lastmodifierdisplayname = "James Vastbinder"
lastmodifieremail = "james@ottemo.io"
date =  "2017-10-24T14:47:14-07:00"
+++

<img src="/images/richkids.png" alt="Example Site" height=300px>
# Developing with Ottemo

Ottemo is a commerce solution born out of the desire to have a fast flexible
stack to speed development. The foundation server is an elegant monolith written
in golang provding a REST api which developers may use to build client
applications for commerce.

Ottemo provides Foundation server binaries and reference stores written in AngularJS,
but any technology that may communicate to a REST backend may be used. As the server
is written in golang, it is hyper efficient regarding resources and even supports
sqlite as a database. Support for mysql and mongodb is also included.  Foundation
may be run on any hardware supported by golang including ARM.

To start developing a commerce site with Ottemo, you should be comfortable with a
frontend technology using javascript or php and talking to a REST api passing json.

In production, Ottemo deploys docker containers to Kubernetes and sessions are stored
in Redis. Developers will also need a way to send out transactional emails, Sendgrid
and MailChimp have solid entry level tiers allowing a site to send out thousands of
emails a month for free.

The goal of this site is to enable developers to quickly set up Ottemo and begin building
a super fast commerce site.
