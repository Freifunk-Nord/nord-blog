---
layout: post
title: Ankündigung - Firmware Update auf Gluon 2016.2.7
---

Moin Freifunk Nord,

wie in der Roadmap vom 16.09.2017 angekündigt steht das Firmware Update auf Gluon 2016.2.7 an.

Sofern es kein wichtiges Update gibt, wird dass dann das letzte Update vor dem Wechsel auf LEDE sein.

Das Update ist zwinged erforderlich, damit ein Wechsel zu LEDE mittels Autoupdater klappt. Daher muss jeder Knotenbetreiber, der nicht schon eine LEDE Firmware nutzt, dieses Update installieren. Was sich geändert hat könnt ihr im Changelog [1] nachlesen. Die Firmware steht bereits auf unser Webseite [2] und auf den Gateways [3] zum download bereit.

Wer für das Update schon jetzt den Autoupdater nutzen möchte, kann dies via SSH mit folgender Befehlszeile tun.

> uci set autoupdater.settings.enabled='1' ; uci set autoupdater.settings.branch='stable' ; uci commit autoupdater ; uci set autoupdater.stable.good_signatures='1' ; autoupdater

Das Update werden wir am Donnerstag den 19.10.2017 aktivieren.

MfG

Christian
Freifunk Nord Admin Team

[1] https://github.com/Freifunk-Nord/nord-site/blob/master/CHANGELOG.md
[2] https://nord.freifunk.net/firmware.html
[3] http://[fd42:eb49:c0b5:4242::fd00]/firmware/stable/sysupgrade/
