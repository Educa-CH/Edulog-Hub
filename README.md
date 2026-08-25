# Edulog-Hub

Der edulog hub ist eine einfache Startseite für häufig genutzte Links. Der Hub kann vorkonfiguriert und so verteilt werden. Der hub dient in erster Linie zum Zusammenstellen von Edulog Links, kann aber auch für weitere Tools und Seiten eingesetzt werden.

## Was kann das Hub?

Du kannst Links als Kacheln speichern und in Gruppen ordnen, zum Beispiel „Schule“, „Tools“ oder „Microsoft“.
Ein Klick auf eine Kachel öffnet die Seite direkt.

Die Kacheln lassen sich per Ziehen mit der Maus verschieben.
Du kannst neue Gruppen und Kacheln hinzufügen oder bestehende wieder löschen.

Alles wird automatisch im Browser gespeichert. Es braucht kein Login und keine Installation.

## Wie verwendet man es?

Lade die Datei "edulog-Hub.html" herunter, speichere sie bspw. auf dem Desktop und öffne die Datei im Browser.

Oben findest du drei Knöpfe:

+ Gruppe erstellt eine neue Kategorie
+ Kachel fügt einen neuen Link hinzu
Reset setzt alles zurück

Wenn du eine Kachel verschieben willst, ziehe sie mit der Maus in die gewünschte Gruppe.

## Erste Einrichtung

Beim ersten Start sind bereits einige Gruppen und Beispiel-Kacheln vorhanden, damit du direkt loslegen kannst.
Du kannst diese im Hub selbst jederzeit ändern oder löschen.

Wenn du die Startwerte anpassen möchtest (zum Beispiel für eine Schule oder Organisation), kannst du das direkt im Code tun.
Dort sind die Standard-Gruppen und Kacheln definiert:

<pre>
/* DEFAULT CONFIG */
const DEFAULT_GROUPS = ["Schule","Microsoft","Admin","Tools"];

const DEFAULT_TILES = [
  { id:"1", name:"Outlook", url:"https://outlook.office.com", group:"Microsoft" },
  { id:"2", name:"Teams", url:"https://teams.microsoft.com", group:"Microsoft" },
  { id:"3", name:"Edulog Lehrmittel", url:"https://digital.lmvz.ch", group:"Schule" }
];
</pre>

Alles, was du hier änderst, erscheint beim ersten Öffnen oder nach einem Reset automatisch im Hub.

Wichtiger Hinweis

Die Daten werden nur auf diesem Gerät im Browser gespeichert.
Wenn der Browser zurückgesetzt wird oder du ein anderes Gerät verwendest, ist das Hub wieder leer.
