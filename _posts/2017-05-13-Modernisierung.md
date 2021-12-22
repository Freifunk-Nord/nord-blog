---
layout: post
title: Modernisierung des Netzes beginnt
---

Hallo Freifunk Nord,

heute beginnen wir mit den Arbeiten zur Netzumstrukturierung. Diese werden sich über die nächsten Tage/Wochen hinziehen, denn wir haben viel vor!

Wie in im Rahmen des Spendenaufrufs angekündigt, ziehen wir die Gateways des Hetzner Servers auf eine neue OVH Plattform um. Dies betrifft auch die Webseite und die dort laufenden Dienste wie Meshviewer und das Knotenformular. Zusammen mit dem Umzug werden wir das Netz auf das neue Routing Protokoll B.A.T.M.A.N. compat 15 umstellen und mit dem Ausrollen des Mesh-Protokolls 802.11s beginnen. Im Rahmen dieser Arbeiten werden wir einige Probleme beseitigen, die derzeit im Netz auftreten. Das fixen der nextnode Adresse und der Wechsel auf ein neues ULA Präfix stehen auf dem Programm. Die Arbeiten sind in mehrere Phasen unterteilt, auf die ich nun kurz eingehen möchte.

Phase 1 - Umzug der Service VM

Die VM, die bisher die Webseite bereitgestellt hat, wird erneuert und bekommt zusätzliche Aufgaben. Neben der Webseite, dem Formular und dem Meshviewer wird die VM auch ein Bein im Freifunk Netz haben und mittels A.L.F.R.E.D. die Statistikdaten erheben. Auch der Zugang zum ICVPN wird zukünftig hierüber realisiert werden. Das spart uns die Synchronisation der Statistikdaten und senkt die Fehleranfälligkeit. Interne Dienste werden dann auch intern geroutet und nicht noch einmal über das VPN geleitet.

Phase 2 - B.A.T.M.A.N. compat 15 Gateways

Im Anschluss werden wir einige Gateways aus dem alten Netz entfernen und auf Debian 8 sowie B.A.T.M.A.N. compat 15 updaten, um damit ein neues Netz aufzuspannen. 

Phase 3 - Firmware Update zum Knotenumzug Teil 1

Alle Router ohne Meshlinks werden im Anschluss via Firmware-Update in das neue Netz verschoben. Gleichzeitig erfolgt der Wechsel auf das Mesh-Protokoll 802.11s. Die Firmware für die neue Domain kann dann bereits von der Webseite und den Gateways manuell heruntergeladen werden, so dass jeder bereits vorher per Hand wechseln kann, wenn er dies möchte.

Phase 4 - Firmware Update zum Knotenumzug Teil 2

Diese Phase erfordert noch etwas Planungsarbeit, da größere Mesh Wolken gezielt geupdated werden müssen, damit keine Router verloren gehen. Diese Phase wird einige Zeit dauern.

Phase 5 - Reduzierung der alten Infrastruktur

Um Nachzügler nicht aus dem Netz auszuschließen, bleibt die alte Infrastruktur noch einige Zeit erhalten, in der dann die verbliebenen Knoten umgezogen werden müssen.

Phase 6 - Abschaltung der alten Infrastruktur

Sobald (so gut wie) alle Knoten im neuen Netz angekommen sind wird das Alte abgeschaltet.

Warum das alles?

Nun es ist Mai, das reicht ja eigentlich schon als Erklärung, nicht! Da wir im Rahmen des Umzugs gut einen 1/3tel der Infrastruktur anfassen müssen, gehen wir nun den Weg bestehendes gleich komplett zu modernisieren und schaffen uns so etwas Luft für die Zukunft. Auch beseitigen wir damit einige Probleme und unterstützen zukünftig mehr Routermodelle. Das rüstet uns gut für die Zukunft.

Wie immer kann es im Rahmen der Arbeit zu Beeinträchtigungen des Netzes und der Dienste kommen. Wir bemühen uns diese gering und kurz zu halten.

Funkt frei!

Gruß
Christian

Freifunk Nord Admin Team
