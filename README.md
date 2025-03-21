Pi-hole Regex Filter - Paranoia Modus

Dieses Repository enthält eine Sammlung von Regex-Filtern für Pi-hole, die das Blockieren von Domains auf die Spitze treiben. Es gibt zwei Hauptdateien:

<a href="https://github.com/rexnox/Raspberrypi/blob/master/Pi-Hole/Regex/all">All-Block Regex/a> → Blockiert alles, was über DNS aufgelöst werden kann. Dies ist ein extremer Paranoia-Modus und sollte mit Bedacht eingesetzt werden.

<a href="https://github.com/rexnox/Raspberrypi/blob/master/Pi-Hole/Regex/Whitelist/ger_rgx_whlist">Deutsche Whitelist (Regex)</a> → Eine Sammlung von regulären Ausdrücken zur gezielten Freigabe von essenziellen Domains für den deutschen Raum.

⚠️ Warnung

Der "All-Block"-Regex-Filter sorgt dafür, dass kein Internetverkehr mehr funktioniert, es sei denn, eine Domain wird explizit freigegeben. Dies ist keine empfohlene Konfiguration für den Alltag, sondern ein Extrem-Setup für besondere Anwendungsfälle.

Nutzung

Block All (Paranoia-Modus aktivieren)

Öffne dein Pi-hole Webinterface.

Navigiere zu Group Management → Adlists.

Füge den Inhalt von all unter Domain-based Blocking → Blacklist ein.

Speichere die Änderungen.

Deutsche Whitelist hinzufügen

Falls du trotz aktiviertem "All-Block" einige essentielle deutsche Dienste nutzen möchtest:

Lade die Regex-Whitelist für den deutschen Raum herunter.

Füge die Einträge unter Domain-based Blocking → Whitelist ein.

Speichere die Änderungen und aktualisiere die Gravity-Listen (pihole -g).
