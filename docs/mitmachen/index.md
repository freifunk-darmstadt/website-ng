# Mitmachen

Klasse, dass du bei uns Mitmischen möchtest! Wir haben hier für dich den typischen Weg zusammengefasst, über den
viele unserer aktiven Community-Mitglieder zu uns gefunden haben.

## Freifunk-Knoten aufstellen
### Einen Freifunk-Knoten bekommen

Das Freifunk-Netz ist ein Mesh-Netzwerk, das von vielen einzelnen Knoten gebildet wird. Als Knoten bezeichnen wir das
Gerät, über welches du ins Freifunk-Netz mit deinem Laptop, Tablet oder Smartphone einsteigst.

!!! note "Freifunk-Knoten"
    Freifunk-Knoten werden oft auch "Freifunk-Router" genannt.

Ein solcher Freifunk-Knoten ist oft ein Handelsüblicher WLAN-Router oder Access-Point, der mit unserer speziellen
Firmware bespielt wird. Unsere Firmware basiert wie die vieler anderer Freifunk-Communities auf
[Gluon](https://www.github.com/freifunk-gluon/gluon).

Wir unterstützen viele verschiedene Geräte, welche du auf unserer Firmware-Seite findest.

Solltest du noch kein kompatibles Gerät besitzen, so haben wir dir auf unserer Webseite auch einen Empfehlungs-Guide
zusammengestellt.

!!! tip "Gebrauchtgeräte"
    Wenn du einen neuen Knoten im Netz von Freifunk Darmstadt betreiben möchtest, so kannst du auch in unserem
    Chat nachfragen, ob jemand vielleicht ein Gerät für dich übrig hat. Oft ziehen Freifunker zum Beispiel zum Ende
    eines Studiums um und haben dann keine Verwendung mehr für ihren Knoten, den sie dir gerne umsonst oder für wenig
    Geld überlassen.

### Firmware installieren

!!! warning "Garantie"
    Die Installation der Firmware auf deinem Gerät kann dazu führen, dass die Garantie des Herstellers erlischt.
    
    Wir übernehmen zwar keine Haftung für Schäden, die durch die Installation unserer Firmware entstehen, aber wir
    helfen dir gerne dabei, deinen Knoten wieder zum Laufen zu bringen, falls etwas schiefgeht.

    Der Prozess ist allerdings in der Regel sehr sicher und einfach, sodass du dir keine Sorgen machen musst.

Hast du einen passenden Router gefunden? Nun musst du diesen mit unserer Firmware bespielen. Da unsere Firmware
Herstellerunabhängig ist, gibt es keine allgemeingültige Anleitung.

1. Solltest du ein Gerät aus unserer Empfehlungsliste gewählt haben, so findest du dort einen direkten Link zur
Anleitung

2. Bei vielen Geräten ist auf unserer Firmware-Seite eine Anleitung verlinkt, die dir Schritt
für Schritt erklärt, wie du die Firmware auf deinem Gerät installierst.

<Bild>



!!! question "Hilfe benötigt?"
    Solltest du Hilfe benötigen, so kannst du dich gerne in unserem Chat melden.

    Falls du zur Installation ein spezielles Kabel benötigst können wir dir dieses oft auch gerne ausleihen.


### Knoten konfigurieren

Nach der Installation der Firmware musst du deinen Knoten noch konfigurieren. Hierbei unterstützt dich unser
Konfigurationsmodus, welcher bei der ersten Inbetriebnahme automatisch startet.

!!! tip "Konfigurationsmodus"
    Ein Freifunk-Knoten hat zwei Betriebsmodi: Den Konfigurationsmodus und den Betriebsmodus. Im Konfigurationsmodus
    kannst du die Einstellungen deines Knotens ändern, im Betriebsmodus ist dein Knoten Teil des Freifunk-Netzes.

    Du erkennst den Konfigurationsmodus daran, dass das Freifunk-Netzwerk in deiner WLAN-Liste fehlt. Bei den
    meisten Geräten blinkt die Status-LED im Konfigurationsmodus gleichmäßig und langsam.

Die folgenden Optionen sind für die meisten Knotenbetreiber die wichtigsten:

- **Knotenname**: Der Name deines Knotens, der im Freifunk-Netz sichtbar ist. Dieser erscheint auch auf der
    Knotenkarte.

- **Mesh-VPN**: Hier kannst du einstellen, ob dein Knoten das Freifunk-Netz über das Internet erreichen soll. Dies ist
    in der Regel sinnvoll, da dein Knoten so auch anderen Knoten im Freifunk-Netz als Internetzugang dient. Die Daten
    werden hierbei niemals direkt über deinen Internetanschluss übertragen, sondern über unsere Server.

    Ebenfalls kannst du ein Limit für die Bandbreite festlegen, welcher dein Knoten maximal verwenden darf.

- **Standort**: Dein Standort, den du auf der Knotenkarte angezeigt haben möchtest. Dies ist wichtig, damit andere
    Nutzer deinen Knoten finden können. Du kannst dich aber auch entscheiden, deinen Standort nicht zu teilen.

- **Kontakt**: Deine Kontaktmöglichkeiten, die auf der Knotenkarte angezeigt werden. Diese sind optional, aber
    empfohlen, falls es Probleme mit deinem Knoten gibt.

Zusätzlich gibt es in den erweiterten Einstellungen noch weitere Optionen, die für fortgeschrittene Nutzer interessant
sind.

- **SSH-Key**: Solltest du dich mit der Materie auskennen, so kannst du hier deinen SSH-Key hinterlegen, um deinen
    Knoten später einfacher zu verwalten.

Wenn du alles eingestellt hast kannst du am Ende der Seite die Einstellungen speichern und deinen Knoten neu starten.

### VPN-Key freischalten

Nachdem du deinen Knoten konfiguriert hast, musst du noch deinen VPN-Key freischalten. Dieser wird benötigt, damit
unsere Server deinen Knoten als Teil des Freifunk-Netzes erkennen.

!!! tip "VPN-Key"
    Den VPN-Key musst du nur einmal freischalten. Solltest du deinen Knoten später erneut in den Konfigurationsmodus
    versetzen, so musst du den VPN-Key nicht erneut freischalten.

Hierfür sendest du uns diesen Key per E-Mail an keys@darmstadt.freifunk.net. Wir schalten deinen Knoten dann so schnell
wie möglich frei.
