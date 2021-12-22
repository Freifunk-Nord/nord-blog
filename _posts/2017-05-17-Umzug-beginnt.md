---
layout: post
title: Umzug in das neue B.A.T.M.A.N. 15 Netz beginnt
---

Moin Freifunk Nord,

die Arbeiten zum Netzaufbau sind nun abgeschlossen und wir beginnen mit dem Umzug der ersten Knoten in das neue Netz. In den nächsten Tagen werden rund 500 Router durch uns automatisch in das neue Netz migriert. In diesem ersten Schritt werden nur Router in das neue Netz wechseln, die keine MESH Verbindung zu anderen Knoten haben. Hierdurch wird verhindert, dass MESH Wolken zerfallen.

Im nächsten Schritt ist dann eure Mithilfe gefragt!

Denn für die restlichen rund 700 Router muss die Update-Reihenfolge per Hand festgelegt werden. Dies erfordert von uns viel Planungsarbeit, damit lokale Wolken nicht abgeschaltet werden. Helft mit, indem ihr eure Router per Hand updatet und uns so Arbeit abnehmt.

Die neue Firmware dafür kann von der Homepage [1] heruntergeladen werden. Auch ein Download direkt von Gateway 1 [2] ist möglich.

Wenn ihr nicht selber updaten, aber trotzdem aktiv mitplanen möchtet, könnt ihr uns an admin@ffnord.net eine Mail schreiben und uns den Knotenname und wenn ihr sie wisst, dessen IPv6 mitteilen. Beachtet dabei immer die Reihenfolge! In einer Meshwolke muss immer erst der äußerste Router zuerst geupdatet werden, dann der nächst äußere usw. bis man am Konten angekommen ist, der die Internetverbindung herstellt.

Gebt bitte unbedingt die Reihenfolge in der Email an:

- Freifunk Router 1
- Freifunk Router 2
- usw.
   
Wer es sich traut, kann auch gerne einen Pull-Request bei Github [3] erstellen und dort seinen Knoten in die "allow" Liste eintragen.
   
Etwa bei 500 Knoten werden wir weitere Gateways in Betrieb nehmen und damit beginnen im alten Netz Server abzuschalten. Dann wird auch der Meshviewer auf das neue Netz zeigen und die Statistik sowie der Knotenalarm wieder aktiviert.
   
Bei Problemen wendet euch bitte direkt via Email an uns oder sucht uns im Chat [4] auf.
   
Funkt Frei!
   
Gruß
   
Christian
Freifunk Nord Admin Team
   
   
[1]   https://nord.freifunk.net/firmware.html
      http://freifunknord.de/firmware/stable/sysupgrade/
[2]   http://vpn1.ffnord/batman15/sysupgrade/
[3]   https://github.com/Freifunk-Nord/nord-bat15-transfer/blob/master/go
[4]   https://riot.eclabs.de/#/room/#ffnord:irc.hackint.org
