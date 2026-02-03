# Freifunk Darmstadt

## Wer seid ihr?

Freifunk Darmstadt ist Teil der Freifunk-Bewegung, welche sich Deutschlandweit für die Verbreitung von freien Netzwerken einsetzt.
Freie Netzwerke sind Netzwerke, welche gemeinschaftlich von Individualpersonen betrieben werden. Diese Netzwerke sind offen für alle
und bieten oftmals freien Zugang zum Internet.

Dies betrifft nicht nur den Netzbetrieb, sondern auch die Software, die wir verwenden. Wir verwenden überall, wo es möglich ist, freie Software
und entwickeln diese weiter. Diese Software ist für jeden frei verfügbar und kann nach belieben angepasst werden.

## Ich will mitmachen!

Wir freuen uns über jede Unterstützung. Da unser Einzugsgebiet sehr groß ist, koordinieren wir uns viel über das Internet.

Bei uns sind alle Menschen willkommen, die sich für freie Netzwerke interessieren.
Egal wo du herkommst, wie alt du bist oder welche Fähigkeiten du hast.
Wenn du deinen <strong>ersten Knoten</strong> aufstellen willst, schau dir gerne unsere [Anleitung für den ersten Freifunk-Knoten](mitmachen/erster-freifunk-knoten.md) an.

Wenn du mit anpacken willst, trete gerne unserem [Chat](https://matrix.to/#/#ffda:hackint.org) und unserem [Forum](https://forum.darmstadt.freifunk.net/) bei.
Wir haben darüber hinaus auch einen Issue-Tracker auf [GitHub](https://github.com/freifunk-darmstadt/projects/issues),
wo wir nicht nur unsere Softwareprojekte verwalten, sondern auch nicht-technische Aufgaben verwalten.


Unser nächstes <strong>Treffen</strong> findet am <strong><span id="next_meet_date">ersten Montag im Monat</span></strong> um <strong>19:30</strong> Uhr statt.
Das Treffen findet im Raum [FreifunkDarmstadtPlenum](https://meet.ffmuc.net/FreifunkDarmstadtPlenum) auf dem Jitsi Meet Server von Freifunk München statt.
Die Teilnahme ist mittels der Jitsi Apps, per Browser sowie über die Telefoneinwahl möglich.
Im [Forum](https://forum.darmstadt.freifunk.net/t/freifunk-treffen-am-13-april-2020-online/847) sind weitere Details zu finden.

<script>
   moment.locale('de');
   
   function getFirstMonday(startDate) {
     // calc date which is the start of isoweek for the month
     var startOfMonth = moment(startDate).utc().startOf('month').startOf('isoweek');
     // add 1 weeks for first monday
     var nextDate = moment(startDate).utc().startOf('month').startOf('isoweek').add(1, 'weeks');
     // if the month from startOfMonth isn't in the previous month (Monday on the 1.), substract one week
     if (nextDate.month() == startOfMonth.month()) {
       nextDate = nextDate.subtract(1, 'weeks');
     }
     return nextDate;
   }
   
   function getNextFirstMonday(startDate) {
     var nextDate = getFirstMonday(startDate);
     // if date is in the past, get next month
     if (nextDate.date() < startDate.date()) {
       nextDate = getFirstMonday(startDate.add(1, 'M'));
     }
     return nextDate;
   }
   
   var currentDate = moment().utc();
   var nextDate = getNextFirstMonday(currentDate);
   
   $('#next_meet_date').text(nextDate.format('DD. MMMM YYYY'));
</script>
