[CCNQ4](http://ccnq.shimaore.net)
=================================

SIP SoftSwitch. All core development is completed (including Voicemail and IP Centrex), development is now focusing on extended applications (such as Call-Center).

Call Processing using Middleware
--------------------------------

CCNQ4 uses the concept of middleware (similar to the ones used by Connect, ExpressJS, ...) to simplify writing dynamic call-handling applications.

* [useful-wind](https://github.com/shimaore/useful-wind), a middleware-based framework to build applications for FreeSwitch.
* [thinkable-ducks](https://github.com/shimaore/thinkable-ducks), a npm package and Docker.IO image extending `useful-wind` with a REST interface and Socket.IO event notifications (to the `spicy-action` proxy); the Docker.IO image embeds FreeSwitch.

Available middlewares / applications:

* [tough-rate](https://github.com/shimaore/tough-rate/), LCR engine; provided as a [Docker image](https://gtihub.com/shimaore/docker.tough-rate) with FreeSwitch, a REST interface and Socket.IO notifications. Also available is [its munin plugin](https://github.com/shimaore/earsplitting-food).
* [huge-play](https://github.com/shimaore/huge-play), the base SBC middleware for CCNQ4.
* [well-groomed-feast](https://github.com/shimaore/well-groomed-feast), the CouchDB-backed voicemail.
* [brown-pencil](https://github.com/shimaore/brown-pencil), an Interactive Voice Service for the French "RIO fixe".
* flat-ornament, parametered execution of data scripts
* earthy-slave, call rating.

Infrastructure
--------------

* [docker.freeswitch](https://github.com/shimaore/docker.freeswitch), [docker.couchdb](https://github.com/shimaore/docker.couchdb), etc. — CCNQ4 relies on docker.io instead of Debian packages which were the norm for CCNQ3.
* [ccnq4-opensips](https://github.com/shimaore/ccnq4-opensips), OpenSIPS-as-Docker-image integrated with configuration, CouchDB interfaces, REST management, ... (includes [royal-thing](https://github.com/shimaore/royal-thing), a tool to automatically restart an OpenSIPS registrant server on changes).
* [willing-toothbrush](https://github.com/shimaore/willing-toothbrush), the CouchDB-backed DNS server.
* [spicy-action](https://github.com/shimaore/spicy-action), a web and Socket.IO proxy to allow browser-side clients, back-ends, and CouchDB, to exchange data.
* [nifty-ground](https://github.com/shimaore/nifty-ground), the distributed sniffer, integrated with `spicy-action`, delivered as a Docker.IO container.
* [ethereal-banana](https://github.com/shimaore/ethereal-banana) and [absurd-clover](https://github.com/shimaore/absurd-clover), browser-side tools to handle sniffer traces and CDR statistics.
* [proud-thumb](https://github.com/shimaore/proud-thumb), demonstration browser tool showing call progress in real-time.
* [nimble-direction](https://github.com/shimaore/nimble-direction), distributed CouchDB toolbox — used to ensure individual call-processing servers continue working even in case of failure or unreachability of the master-master, main provisioning database.
* [cuddly](https://github.com/shimaore/cuddly), a devops notification framework, simple to use and deploy, based on Socket.IO.
* [gabby-potato](https://github.com/shimaore/tough-rate/), a Socket.IO-controlled FreeSwitch instance meant to be used as a generic client emulator and call-generator for automated testing.
* rightful-hot-server, app conventions for RioJS+ZappaJS — server-side.
* rightful-hot, app conventions for RiotJS+ZappaJS — client-side.
* rough-produce, log support events.
* fr-sounds, French audio files for FreeSwitch, along with ordinary-tail, audio files for new services.
* 2015-rmll-isp, a presentation about voice for ISP (in French).
* incomplete: calm-belief, voicemail database cleanups.
* ~exultant-sounds~, click-to-dial over socket.io → now part of huge-play.
* zesty-vessel, socket-to-mail service.
* spicy-action-user, user parameters (locale, timezone) for spicy-action.
* charming-circle, per-user database (for voicemail, provisioning, …).
* astonishing-competition, CDR aggregation (pre-invoicing).
* numbering-plans, International Numbering Plans.
* entertaining-crib, CDR rating.
* chunky-grade, provisioning validation.
* frantic-team, inject replication documents in CouchDB.

FreeSwitch XML Configuration
----------------------------

* [acoustic-line](https://github.com/shimaore/acoustic-line), the CoffeeScript templating system used to generate FreeSwitch XML configurations.
* [bumpy-lawyer](https://github.com/shimaore/bumpy-lawyer), FreeSwitch phrases for pronunciation of numbers, spelling words, etc.

FreeSwitch interaction with Node.js
-----------------------------------

* [esl](https://github.com/shimaore/esl), the Node.js Promise-based interface to FreeSwitch's event socket (inbound and outbound).
