[CCNQ4](http://ccnq.shimaore.net)
=================================

SIP SoftSwitch. The development has started, see:
* [tough-rate](https://github.com/shimaore/tough-rate/), the new, middleware-based, LCR engine, provided as a [Docker image](https://gtihub.com/shimaore/docker.tough-rate) with FreeSwitch, a web interface and notifications. Also available is [its munin plugin](https://github.com/shimaore/earsplitting-food)).
* [acoustic-line](https://github.com/shimaore/acoustic-line), a CoffeeScript templating system to generate FreeSwitch XML configurations.
* [esl](https://github.com/shimaore/), a Promise-based interface to FreeSwitch's event socket (inbound and outbound).
* [docker.freeswitch](https://github.com/shimaore/docker.freeswitch), [docker.couchdb](https://github.com/shimaore/docker.couchdb), etc. -- ccnq4 will rely on docker.io instead of Debian packages which were the norm for ccnq3.
* [spicy-action](https://github.com/shimaore/spicy-action) is a web an] Socket.IO proxy to allow clients, back-ends, and CouchDB, to exchange data.
* [nifty-ground](), the sniffer trace tool, integrated with `spicy-action`, delivered as a Docker.IO container.
* [useful-wind](https://github.com/shimaore/useful-wind), a middleware-based framework to build applications for FreeSwitch.
* [thinkable-ducks](https://github.com/shimaore/thinkable-ducks), a Docker.IO image that extends `useful-wind` with a web interface and event notifications (to the `spicy-action` proxy) and embeds FreeSwitch.
* [abstracted-birds](https://github.com/shimaore/abstracted-birds) offers some ideas to build a UI for ccnq4 (using KnockoutJS and Browserify, via the [kow](https://github.com/shimaore/kow) widget constructor). It handles LCR rules.
* [ethereal-banana](https://github.com/shimaore/ethereal-banana) and [absurd-clover](https://github.com/shimaore/absurd-clover), the former CCNQ3 (browser-side) tools to handle sniffer traces and CDR statistics, ported to CCNQ4.
* [royal-thing](https://github.com/shimaore/royal-thing), a tool to automatically restart an OpenSIPS registrant server on changes.
And more to come!
<!-- * [well-groomed-feast](https://github.com/shimaore/well-groomed-feast), the new voicemail server (current under development). -->
<!-- * [squealing-cow] -->
<!-- * [huge-play] -->
