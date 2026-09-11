# SKILL.md — Deutsche Firmenwebsite: Recht, Datenschutz, Accessibility, Security & Launch

## Zweck

Diese Skill-Datei steuert Claude beim Planen, Entwickeln, Prüfen und Ausliefern einer Firmenwebsite für ein in Deutschland tätiges Unternehmen.

Ziel: Eine technisch saubere, datenschutzbewusste, barrierearme/barrierefreie und rechtlich möglichst belastbare Website erstellen, ohne Rechtslage, Unternehmensdaten, Anbieterbedingungen oder Tatsachen zu erfinden.

**Wichtig:** Diese Skill-Datei ersetzt keine individuelle Rechtsberatung. Bei erheblichen Risiken, regulierten Branchen, Verträgen, Abmahnrisiken, Datenschutz-Folgenabschätzungen oder unklarer Rechtslage muss Claude ausdrücklich auf anwaltliche bzw. fachliche Prüfung hinweisen.

---

## 1. Grundregeln für Claude

1. Arbeite nach deutschem Recht und berücksichtige EU-Recht, soweit es für die Website relevant ist.
2. Bei Rechtsfragen immer den aktuellen Stand zum Projektzeitpunkt prüfen. Nutze bevorzugt Primärquellen wie `gesetze-im-internet.de`, EUR-Lex, BfDI/Datenschutzaufsichtsbehörden, Bundesministerien und offizielle Stellen.
3. Behaupte nie, dass eine Website „100 % rechtssicher“ sei. Verwende stattdessen Formulierungen wie „rechtlich zu prüfen“, „nach aktuellem Prüfstand“ oder „unter den genannten Annahmen“.
4. Erfinde niemals Firmendaten, Handelsregisternummern, USt-ID, Anschrift, Aufsichtsbehörde, Berufsbezeichnung, Datenschutzbeauftragten, Preise, Zertifikate, Kunden, Referenzen oder sonstige Tatsachen.
5. Verwende für rechtliche Platzhalter eindeutig erkennbare Tokens, z. B. `[FIRMENNAME]`, `[ANSCHRIFT]`, `[UST-ID]`.
6. Keine juristischen Texte aus fremden Websites kopieren. Inhalte individuell erstellen bzw. anhand offizieller Quellen und der tatsächlichen Website konfigurieren.
7. Jede Datenschutzangabe muss mit dem realen technischen Verhalten übereinstimmen.
8. Jede externe Ressource prüfen: Fonts, Analytics, Maps, Video, Captcha, CDN, Chat, Social Plugins, Consent-Tools, APIs, Zahlungsdienste usw.
9. Bei Unsicherheit nicht raten. Entweder Primärquelle prüfen oder die Unsicherheit klar markieren.
10. Nach Änderungen immer erneut prüfen, welche rechtlichen Folgen die Änderung hat.

---

# 2. Zielprofil: typische Firmenwebsite

Diese Skill-Datei gilt standardmäßig für eine klassische Unternehmenswebsite, z. B.:

- Startseite
- Leistungen
- Über uns
- Team
- Projekte/Referenzen
- Kontakt
- Impressum
- Datenschutz
- ggf. Blog/News

Sie ist **nicht automatisch ausreichend** für:

- Online-Shop
- Marktplatz
- Nutzerforum
- soziale Plattform
- medizinische Leistungen
- Finanz-/Versicherungsangebote
- Glücksspiel
- stark regulierte Produkte
- Dating-/Minderjährigenangebote
- umfangreiche Nutzerprofile
- KI-Systeme mit besonderen regulatorischen Pflichten

In diesen Fällen müssen zusätzliche Rechtsmodule aktiviert und separat geprüft werden.

---

# 3. Pflicht- und Prüfschichten

Bei jeder Firmenwebsite muss Claude mindestens diese Schichten prüfen:

1. Anbieterkennzeichnung / Impressum
2. Datenschutz / DSGVO
3. Cookies / Endgerätezugriff / TDDDG
4. Urheberrecht / Medienrechte / Bildrechte / Musik / Fonts / Icons
5. Markenrecht und Wettbewerbsrecht
6. Barrierefreiheit und BFSG/BFSGV, soweit anwendbar
7. IT-Sicherheit
8. Formulare und Kommunikation
9. externe Dienste und Datenübermittlungen
10. Tracking/Analytics/Marketing
11. Hosting, Server und Logs
12. geschäftliche Inhalte, Preise und Werbeaussagen
13. branchenspezifisches Recht
14. Release-/Launch-Prüfung

---

# 4. Primäre Rechtsquellen

Bei einer deutschen Firmenwebsite sind insbesondere folgende Quellen zu prüfen:

- Digitale-Dienste-Gesetz (DDG), insbesondere § 5
- Datenschutz-Grundverordnung (DSGVO), insbesondere Art. 5, 6, 7, 12–15, 17–22, 25, 28, 30, 32 und je nach Fall Art. 35
- Bundesdatenschutzgesetz (BDSG), soweit ergänzend anwendbar
- Telekommunikation-Digitale-Dienste-Datenschutz-Gesetz (TDDDG), insbesondere § 25
- Bürgerliches Gesetzbuch (BGB), je nach Funktion/Vertrag
- Einführungsgesetz zum Bürgerlichen Gesetzbuche (EGBGB)
- Gesetz gegen den unlauteren Wettbewerb (UWG)
- Preisangabenverordnung (PAngV), wenn gegenüber Verbrauchern Preise angegeben werden
- Urheberrechtsgesetz (UrhG)
- Kunsturhebergesetz (KunstUrhG), insbesondere § 22 für Bildnisse
- Markengesetz (MarkenG)
- Medienstaatsvertrag (MStV), soweit journalistisch-redaktionelle Angebote bzw. entsprechende Verantwortlichkeit vorliegt
- Barrierefreiheitsstärkungsgesetz (BFSG)
- Verordnung zum Barrierefreiheitsstärkungsgesetz (BFSGV)
- ggf. Digital Services Act (EU-Verordnung 2022/2065) bei Plattform-/Hosting-Funktionen
- branchenspezifische Gesetze und Verordnungen

**Keine pauschale Aussage treffen, dass jede dieser Normen auf jede Firmenwebsite anwendbar ist.** Immer Anwendungsbereich prüfen.

---

# 5. Impressum / Anbieterkennzeichnung

## Rechtsgrundlage

Für geschäftsmäßige digitale Dienste sind insbesondere die Informationspflichten des § 5 DDG zu prüfen.

Das Impressum muss leicht erkennbar, unmittelbar erreichbar und ständig verfügbar sein.

## Prüfung

Je nach Unternehmen/Fall müssen unter anderem geprüft werden:

- vollständiger Name/Firma
- ladungsfähige Anschrift
- Rechtsform
- vertretungsberechtigte Person(en)
- schnelle elektronische Kontaktaufnahme
- E-Mail-Adresse
- ggf. weitere unmittelbare Kommunikationsmöglichkeit
- Handelsregister/anderes Register
- Registergericht
- Registernummer
- ggf. Umsatzsteuer-Identifikationsnummer
- ggf. Wirtschafts-Identifikationsnummer
- ggf. zuständige Aufsichtsbehörde
- ggf. berufsrechtliche Angaben
- ggf. Kammer
- ggf. Berufsbezeichnung
- ggf. Staat der Verleihung
- ggf. berufsrechtliche Regelungen und deren Fundstelle
- ggf. besondere Angaben bei audiovisuellen Mediendiensten
- ggf. Abwicklungs-/Liquidationshinweis

## Umsetzung

Im Footer muss mindestens ein direkt erreichbarer Link „Impressum“ stehen.

Keine:

- versteckten Links
- unklaren Sammelbegriffe wie „Info“ statt eindeutigem Zugang
- Fantasieangaben
- Postfach als Ersatz für eine erforderliche ladungsfähige Anschrift

---

# 6. Datenschutz: DSGVO

## Grundprinzip

Claude muss zuerst den tatsächlichen Datenfluss ermitteln und erst danach die Datenschutzerklärung formulieren.

## Zu inventarisieren

Erstelle vor dem Launch eine Datenflussliste mit:

| Verarbeitung | Daten | Zweck | Rechtsgrundlage | Empfänger | Speicherfrist | Drittland? | Consent? |
|---|---|---|---|---|---|---|---|

Beispiele:

- Server-Logs
- Kontaktformular
- E-Mail-Kommunikation
- Newsletter
- Analytics
- Marketing
- Maps
- Videos
- Fonts
- Captcha
- CRM
- Terminbuchung
- Cloudspeicher
- Support-/Chat-System

## Datenschutzerklärung

Je nach tatsächlicher Verarbeitung sind u. a. zu erläutern:

- Verantwortlicher
- Kontaktdaten
- ggf. Datenschutzbeauftragter
- Kategorien personenbezogener Daten
- Zwecke
- Rechtsgrundlagen
- berechtigte Interessen, falls Art. 6 Abs. 1 lit. f DSGVO verwendet wird
- Empfänger/Kategorien von Empfängern
- Übermittlungen in Drittländer
- geeignete Garantien, soweit erforderlich
- Speicherdauer oder Kriterien für deren Bestimmung
- Rechte betroffener Personen
- Widerrufsmöglichkeiten
- Widerspruchsrecht
- Beschwerderecht bei der Aufsichtsbehörde
- ggf. automatisierte Entscheidungsfindung/Profiling
- ggf. Pflicht zur Bereitstellung und Folgen der Nichtbereitstellung
- Quellen der Daten, wenn sie nicht beim Betroffenen erhoben wurden

## Datenminimierung

Nur notwendige Daten erheben.

Beispiel Kontaktformular:

```html
<label for="name">Name</label>
<input id="name" name="name" autocomplete="name" required>

<label for="email">E-Mail-Adresse</label>
<input id="email" name="email" type="email" autocomplete="email" required>

<label for="message">Nachricht</label>
<textarea id="message" name="message" required></textarea>
```

Nicht ohne sachlichen Grund:

- Geburtsdatum
- private Telefonnummer
- Adresse
- Geschlecht
- besondere Kategorien personenbezogener Daten

abfragen.

---

# 7. Rechtsgrundlagen richtig behandeln

Claude darf niemals automatisch „Einwilligung“ als Universal-Rechtsgrundlage einsetzen.

Für jeden Verarbeitungsvorgang prüfen:

- Art. 6 Abs. 1 lit. a DSGVO — Einwilligung
- Art. 6 Abs. 1 lit. b DSGVO — Vertrag / vorvertragliche Maßnahmen
- Art. 6 Abs. 1 lit. c DSGVO — rechtliche Verpflichtung
- Art. 6 Abs. 1 lit. d DSGVO — lebenswichtige Interessen
- Art. 6 Abs. 1 lit. e DSGVO — öffentliche Aufgabe
- Art. 6 Abs. 1 lit. f DSGVO — berechtigtes Interesse

Bei besonderen Kategorien personenbezogener Daten zusätzlich Art. 9 DSGVO prüfen.

---

# 8. Consent / Einwilligung

Eine wirksame Einwilligung muss insbesondere:

- freiwillig
- für den konkreten Fall
- informiert
- unmissverständlich
- durch aktive Handlung
- widerrufbar

sein.

Keine vorangekreuzten Einwilligungen verwenden.

Keine Einwilligung in allgemeiner Form für völlig unterschiedliche Zwecke erzwingen.

---

# 9. Cookies und TDDDG § 25

## Grundregel

Vor dem Speichern von Informationen in der Endeinrichtung oder dem Zugriff auf bereits gespeicherte Informationen prüfen, ob § 25 TDDDG greift.

Einwilligung ist nach § 25 Abs. 1 TDDDG grundsätzlich erforderlich, außer eine gesetzliche Ausnahme greift.

Nach § 25 Abs. 2 TDDDG ist eine Einwilligung insbesondere nicht erforderlich, wenn der Zweck allein die Übertragung einer Nachricht über ein öffentliches Telekommunikationsnetz ist oder die Speicherung/der Zugriff unbedingt erforderlich ist, um einen vom Nutzer ausdrücklich gewünschten digitalen Dienst bereitzustellen.

## Technische Regel

Consent-gesteuerte Skripte dürfen erst geladen werden, wenn die erforderliche Einwilligung vorliegt.

Unbedingt erforderliche Technologien dürfen nicht fälschlich als Marketing- oder Statistik-Technologien kategorisiert werden.

## Consent-Banner

Ein plausibles Basismodell:

- Alle akzeptieren
- Ablehnen / Nur notwendige
- Einstellungen

Nutzer darf nicht durch irreführende Gestaltung zur Zustimmung gedrängt werden.

## Consent-Management muss können

- Kategorien darstellen
- konkrete Zwecke darstellen
- Anbieter darstellen
- Einwilligungsstatus speichern
- Einwilligungswiderruf ermöglichen
- Status ändern können
- Nachweis/Protokollierung ermöglichen, soweit erforderlich

---

# 10. Consent-freie Alternative

Wenn möglich und sinnvoll:

- selbst gehostete Fonts
- datensparsame Analytics-Lösung
- serverseitige/statistikbasierte Alternativen
- keine unnötigen Third-Party-Tracker
- direkte Links statt eingebetteter Social Plugins

Ziel: so wenig personenbezogene Daten und Drittanbieter wie möglich.

---

# 11. Externe Dienste: Pflichtprüfung

Für jede externe Ressource eine Inventarliste führen:

| Dienst | Kategorie | Daten | Ziel | geladen wann? | Rechtsgrundlage | Consent? | AVV? | Drittland? |
|---|---|---|---|---|---|---|---|---|

Prüfen insbesondere:

- Google Fonts
- Google Maps
- YouTube
- Vimeo
- Google Analytics
- Meta Pixel
- LinkedIn Insight Tag
- TikTok Pixel
- Hotjar/Session Recording
- reCAPTCHA
- hCaptcha
- Cloudflare
- CDN
- externe Chatdienste
- Terminbuchung
- Newsletter
- CRM
- Zahlungsdienstleister

Keine Einbindung nur deshalb, weil sie „Standard“ ist.

---

# 12. Google Fonts

Bevorzugt selbst hosten, wenn kein sachlicher Grund für externe Bereitstellung besteht.

Keine unnötige Übertragung von Besucher-IP-Adressen an Drittanbieter nur für Schriftarten.

---

# 13. Analytics / Tracking

Vor Aktivierung prüfen:

1. Zweck
2. technische Funktionsweise
3. Cookies/Storage
4. personenbezogene Daten
5. IP-Verarbeitung
6. Fingerprinting
7. Profiling
8. Empfänger
9. Drittlandtransfer
10. Rechtsgrundlage
11. Consent
12. Widerruf
13. Aufbewahrung
14. Datenschutzerklärung

Keine Tracking-Bibliothek in `index.html` laden, bevor notwendige Zustimmung vorliegt.

---

# 14. Formulare

Für jedes Formular prüfen:

- Zweck
- Datenminimierung
- Pflicht-/optionale Felder
- Validierung
- Fehlermeldungen
- Datenschutz-Hinweis
- sichere Übertragung
- Spam-Schutz
- CSRF-Schutz, sofern serverseitig relevant
- sichere Speicherung
- Löschkonzept
- E-Mail-Versand

Keine personenbezogenen Daten in URLs übertragen, wenn vermeidbar.

---

# 15. E-Mail / Kontaktanfragen

Prüfen:

- sichere Verbindung
- verantwortlicher Empfänger
- Weiterleitung
- Drittanbieter-Mailhost
- Auftragsverarbeitung, falls relevant
- Aufbewahrung
- Löschung
- automatische Antworttexte

Keine sensiblen Informationen unnötig in automatischen E-Mail-Antworten wiederholen.

---

# 16. Newsletter

Nur aktivieren, wenn tatsächlich benötigt.

Prüfen:

- geeignete Rechtsgrundlage
- Double-Opt-In
- Einwilligungsnachweis
- Abmeldemöglichkeit
- Anbieter
- AVV/Datenschutzvereinbarung, soweit erforderlich
- Drittlandtransfer
- Datenschutzerklärung
- Werberecht nach UWG

---

# 17. Werbung / UWG

Keine irreführenden Aussagen.

Claims wie:

- „Nr. 1“
- „bester Anbieter“
- „garantiert“
- „100 % sicher“
- „klimaneutral“
- „zertifiziert“
- „Testsieger“
- „nur heute“
- „begrenztes Angebot"

dürfen nicht erfunden oder unbelegt verwendet werden.

Bei vergleichender Werbung, Rankings, Gütesiegeln, Nutzerbewertungen und Umweltclaims besondere Prüfung durchführen.

---

# 18. Fake Knappheit und Dark Patterns

Nicht verwenden:

- gefälschte Countdown-Timer
- gefälschte Lagerbestände
- erfundene Besucherzahlen
- erfundene Käufe
- künstlich versteckte Ablehnung
- irreführende Buttons
- absichtlich schwer auffindbare Kündigung/Widerrufsmöglichkeiten

---

# 19. Bilder und Fotografien

Für jedes Bild muss die Nutzungsberechtigung feststehen.

Quellen dokumentieren:

- eigenes Foto
- lizenzierter Stock
- Creative Commons / konkrete Lizenz
- Rechteübertragung
- Kundenfreigabe
- Agenturvertrag

Dokumentiere bei gekauften Bildern:

- Quelle
- Lizenz
- Kaufdatum
- erlaubte Nutzung
- Bearbeitungsrechte
- kommerzielle Nutzung
- Namensnennungspflicht

---

# 20. Personenfotos

Vor Veröffentlichung von Personenbildern Rechtsgrundlage und Einwilligungssituation prüfen.

§ 22 KunstUrhG beachten; gesetzliche Ausnahmen separat prüfen.

Besonders sauber arbeiten bei:

- Mitarbeiterportraits
- Kundenfotos
- Events
- Minderjährigen
- Testimonials

Nie einfach annehmen, dass eine Aufnahme automatisch zur Website-Veröffentlichung berechtigt.

---

# 21. Urheberrecht

Prüfen:

- Fotos
- Illustrationen
- Icons
- Videos
- Musik
- Texte
- Animationen
- Code
- Templates
- Fonts

Das öffentliche Online-Bereitstellen kann urheberrechtlich relevante Nutzungen darstellen.

Quelle allein ist nicht gleich Lizenz.

„Im Internet gefunden“ ist keine Nutzungserlaubnis.

---

# 22. Open Source / npm / Libraries

Für jede externe Library prüfen:

- Lizenz
- Versionsnummer
- Herkunft
- Integrität
- Wartungsstatus
- bekannte Sicherheitslücken
- Lizenzpflichten

Typische Lizenzen:

- MIT
- BSD
- Apache-2.0
- GPL
- LGPL
- MPL
- proprietär

Bei Copyleft-Lizenzen besondere Prüfung.

---

# 23. Icons / Fonts / Assets

Keine Assets ungeprüft aus Google Images, Pinterest oder zufälligen Websites übernehmen.

Für jede Ressource:

- Herkunft
- Lizenz
- kommerzielle Nutzung
- Modifikation
- Attribution

prüfen.

---

# 24. Marken

Keine Markenidentität imitieren und keine falsche Partnerschaft suggerieren.

Nicht schreiben:

> offizieller Partner von [MARKE]

ohne reale Berechtigung.

Drittfirmen, Logos und Marken nur im notwendigen und zulässigen Umfang verwenden.

---

# 25. Barrierefreiheit / BFSG

Seit 28. Juni 2025 ist das BFSG für bestimmte Produkte und Dienstleistungen relevant.

Prüfen, ob die konkrete Firmenwebsite eine vom BFSG erfasste Dienstleistung des elektronischen Geschäftsverkehrs anbietet.

Für Kleinstunternehmen, die Dienstleistungen anbieten/erbringen, besteht nach § 3 Abs. 3 BFSG eine gesetzliche Ausnahme von Absatz 1; trotzdem sollte die Website möglichst barrierearm umgesetzt werden.

Nicht pauschal behaupten, dass jede Firmenwebsite BFSG-pflichtig ist.

---

# 26. Accessibility-Engineering

Als technische Mindestbasis orientiert sich Claude an WCAG 2.2, sofern kein speziellerer Standard vorgegeben ist.

Prüfen:

### Wahrnehmbar

- Alt-Texte
- ausreichender Kontrast
- sichtbare Überschriftenhierarchie
- keine Informationen nur über Farbe
- responsive Inhalte
- Zoom
- skalierbarer Text

### Bedienbar

- Tastaturbedienung
- sichtbarer Fokus
- ausreichende Klickflächen
- keine Tastaturfallen
- sinnvoller Tabfluss
- Skip-Link
- Navigation konsistent

### Verständlich

- verständliche Sprache
- eindeutige Fehlermeldungen
- Labels
- Instruktionen
- konsistente Navigation

### Robust

- semantisches HTML
- ARIA nur wenn nötig
- korrekte Rollen/Zustände
- Screenreader-Kompatibilität

---

# 27. Semantisches HTML

Bevorzugen:

```html
<header>...</header>
<nav aria-label="Hauptnavigation">...</nav>
<main>
  <h1>...</h1>
  <section>
    <h2>...</h2>
  </section>
</main>
<footer>...</footer>
```

Nicht alles mit `<div>` bauen, wenn eine semantische Struktur existiert.

---

# 28. Bilder

Beispiel:

```html
<img
  src="/images/team.jpg"
  alt="Das fünfköpfige Team von [FIRMENNAME] im Büro"
  width="1600"
  height="1000"
>
```

Dekorative Bilder:

```html
<img src="/images/deko.svg" alt="" aria-hidden="true">
```

Alt-Text soll den Zweck/Inhalt vermitteln, nicht einfach Dateiname sein.

---

# 29. Formulare: Accessibility

Jedes relevante Feld bekommt ein Label.

```html
<label for="email">E-Mail-Adresse</label>
<input id="email" name="email" type="email" autocomplete="email" aria-describedby="email-hint">
<p id="email-hint">Wir verwenden Ihre E-Mail-Adresse nur zur Bearbeitung Ihrer Anfrage.</p>
```

Fehler müssen programmatisch erfassbar und verständlich sein.

---

# 30. Keyboard Testing

Vor Release:

- nur Tastatur verwenden
- Tab-Reihenfolge prüfen
- Shift+Tab prüfen
- Enter/Space prüfen
- Escape prüfen
- Fokus in Dialogen prüfen
- Cookie-Banner prüfen
- Mobile-Menü prüfen
- Formular prüfen

---

# 31. Responsive Design

Mindestens testen:

- Smartphone klein
- Smartphone groß
- Tablet
- Laptop
- Desktop
- breite Desktop-Auflösung
- Zoom mindestens 200 %, soweit für den jeweiligen Standard relevant

Keine Inhalte dürfen horizontal unerreichbar werden, sofern dies nicht sachlich erforderlich ist.

---

# 32. Datenschutzfreundliche Default-Konfiguration

Default:

- keine unnötigen Tracker
- keine unnötigen Third-Party-Skripte
- keine unnötigen Cookies
- keine unnötigen Fonts von Drittservern
- keine unnötigen eingebetteten Social Widgets
- minimale Serverdaten
- sichere Header

---

# 33. HTTPS / TLS

Produktivwebsite grundsätzlich über HTTPS ausliefern.

Prüfen:

- gültiges Zertifikat
- HTTP → HTTPS Redirect
- keine Mixed Content Ressourcen
- sichere Cookies
- HSTS nach sinnvoller Prüfung
- TLS-Konfiguration aktuell

Keine sensiblen Formulare über HTTP übertragen.

---

# 34. HTTP Security Headers

Je nach Hosting/Architektur prüfen:

- Content-Security-Policy
- Strict-Transport-Security
- X-Content-Type-Options
- Referrer-Policy
- Permissions-Policy
- Frame-Anforderungen / `frame-ancestors`

Keine Header blind kopieren. Vor CSP besonders externe Ressourcen inventarisieren.

---

# 35. XSS

Alle dynamischen Inhalte kontextgerecht escapen/sanitizen.

Kein blindes:

```js
container.innerHTML = userInput;
```

Bei HTML-Generierung aus Nutzereingaben sichere Sanitization verwenden.

---

# 36. CSRF

Bei zustandsändernden serverseitigen Aktionen prüfen:

- CSRF-Schutz
- SameSite-Cookies
- Origin/Referer-Prüfung, wo geeignet
- sichere Sessionverwaltung

---

# 37. SQL Injection

Niemals SQL per Stringverkettung aus Nutzereingaben bauen.

Bevorzugen:

- Prepared Statements
- sichere ORM-Abfragen
- serverseitige Validierung

---

# 38. Passwörter

Bei Kunden-/Admin-Logins:

- nie Klartext speichern
- moderne Passwort-Hashing-Verfahren verwenden
- sichere Sessionverwaltung
- Rate Limiting
- MFA für Admins möglichst aktivieren
- Passwort-Reset absichern
- keine Geheimnisse im Frontend

---

# 39. Secrets

Niemals in Git/Frontend:

- API Keys mit Schreibrechten
- Datenbankpasswörter
- SMTP-Passwörter
- OAuth Secrets
- private Tokens
- Cloud Credentials

Umgebungsvariablen und Secret Management nutzen.

---

# 40. Backups

Produktivsysteme brauchen je nach Bedeutung:

- Backups
- getestete Wiederherstellung
- getrennte Sicherungen
- Zugriffsbegrenzung
- Verschlüsselung, soweit angemessen
- dokumentierte Aufbewahrung

Ein Backup, dessen Restore nie getestet wurde, ist kein verlässlich geprüfter Backup-Prozess.

---

# 41. Server-Logs

Prüfen:

- welche Logdaten entstehen
- IP-Adressen
- Zeitpunkte
- User-Agent
- Fehlerdaten
- Zugriffe
- Log-Aufbewahrung
- Zugriff auf Logs
- ggf. Datenschutzinformation

Keine unnötig langen Aufbewahrungszeiten.

---

# 42. Hosting / Auftragsverarbeitung

Prüfen:

- Anbieter
- Rechenzentrum
- Datenstandort
- Auftragsverarbeitung gemäß Art. 28 DSGVO, wenn einschlägig
- Unterauftragsverarbeiter
- technische Maßnahmen
- Drittlandbezug
- Lösch-/Rückgabekonzept

---

# 43. Drittlandtransfers

Wenn personenbezogene Daten aus der EU/EWR in Drittländer fließen, prüfen:

- Zielland
- Angemessenheitsbeschluss
- geeignete Garantien
- Standardvertragsklauseln, falls erforderlich
- zusätzliche Maßnahmen
- konkrete Anbieter-/Datenflüsse

Nicht automatisch behaupten, dass ein US-Anbieter „DSGVO-konform“ ist, ohne aktuelle Prüfung.

---

# 44. Auftragsverarbeiter

Typische Kandidaten:

- Hosting
- E-Mail/Cloud
- CRM
- Newsletter
- Terminbuchung
- Support
- Analytics
- externe Formularsysteme

Prüfen, ob Art. 28 DSGVO einschlägig ist und welche Verträge/Unterlagen erforderlich sind.

---

# 45. Verzeichnis von Verarbeitungstätigkeiten

Wenn Art. 30 DSGVO anwendbar ist, Unternehmensprozesse dokumentieren.

Für Website-Projekte mindestens die relevanten Prozesse beschreiben:

- Kontaktanfragen
- Newsletter
- Analytics
- Kundenverwaltung
- Terminbuchung
- Serverbetrieb
- Bewerbungen, falls vorhanden

---

# 46. Löschkonzept

Für jede personenbezogene Datenart festlegen:

- warum sie gespeichert wird
- maximale/angemessene Aufbewahrung
- Löschereignis
- Löschprozess
- Ausnahmen wegen gesetzlicher Aufbewahrung

Keine pauschale „wir löschen alles nach X Tagen“-Aussage, wenn der Prozess dies nicht wirklich tut.

---

# 47. Datenschutzrechte

Website muss je nach Fall Informationen über folgende Rechte korrekt abbilden:

- Auskunft
- Berichtigung
- Löschung
- Einschränkung
- Datenübertragbarkeit
- Widerspruch
- Widerruf
- Beschwerde

Keine unzutreffenden Aussagen über Fristen oder Rechte.

---

# 48. Journalistischer/redaktioneller Inhalt

Bei Blog, Magazin, News oder anderen redaktionellen Angeboten prüfen:

- MStV
- Verantwortliche Person für journalistisch-redaktionelle Angebote, soweit erforderlich
- ggf. weitere medienrechtliche Vorgaben

Keine erfundene „Redaktion“.

---

# 49. Testimonials / Referenzen / Kundenlogos

Vor Veröffentlichung prüfen:

- tatsächliche Kundenbeziehung
- Erlaubnis zur Nutzung von Namen/Logo
- Inhaltliche Wahrheit
- Aktualität
- Nutzungsdauer

Keine erfundenen Kunden.

---

# 50. Preise auf Firmenwebsites

Wenn gegenüber Verbrauchern Preise für Waren/Leistungen genannt werden, PAngV prüfen.

Insbesondere:

- Gesamtpreis
- relevante Grundpreisangaben
- Klarheit
- ggf. Umsatzsteuerhinweise
- ggf. Versandkosten
- Preisermäßigungen und 30-Tage-Referenzpreis gemäß § 11 PAngV

Bei reinem B2B-Angebot die konkrete Anwendbarkeit prüfen statt PAngV pauschal zu behaupten.

---

# 51. Wenn die Firmenwebsite doch Verträge abschließt

Sobald die Seite:

- Leistungen direkt bucht
- Bestellungen entgegennimmt
- Abos verkauft
- digitale Inhalte verkauft
- Onlinekurse verkauft
- Shopfunktionen besitzt

muss Claude zusätzliche Verbraucher- und Vertragsregeln prüfen.

Insbesondere können relevant sein:

- Informationspflichten
- Widerrufsrecht
- Muster-Widerrufsformular
- Bestellübersicht
- § 312j BGB
- Button-Lösung
- Kündigungsfunktionen, soweit gesetzlich erforderlich
- seit Juni 2026 geltende Regeln zur elektronischen Widerrufsfunktion, soweit der konkrete Vertrag darunter fällt

Nicht auf eine reine Firmenwebsite übertragen, wenn dort gar kein Vertrag online geschlossen wird.

---

# 52. Online-Shop / Checkout-Modul

Nur aktivieren, wenn tatsächlich ein Shop gebaut wird.

Prüfen:

- Vertragsgegenstand
- Preise
- Versandkosten
- Lieferzeiten
- Zahlarten
- Bestellprozess
- Lieferbeschränkungen
- wesentliche Eigenschaften
- Widerruf
- gesetzliche Gewährleistungsrechte
- Zahlungsbutton
- Bestellbestätigung
- AGB, falls verwendet
- Datenschutzerklärung
- Consent
- Barrierefreiheit

§ 312j BGB verlangt bei zahlungspflichtigen Online-Verbraucherverträgen eine klar erkennbare Zahlungspflicht; der Button muss grundsätzlich mit „zahlungspflichtig bestellen“ oder einer entsprechend eindeutigen Formulierung beschriftet sein.

---

# 53. Widerruf / Kündigung

Nicht auf jeder Firmenwebsite erforderlich.

Wenn online Verbraucher-Verträge geschlossen werden, konkrete Vertragssituation prüfen.

§ 355 BGB sieht grundsätzlich eine 14-tägige Widerrufsfrist vor, wenn das gesetzliche Widerrufsrecht besteht; Beginn, Ausnahmen und Folgen hängen vom Vertrag ab.

Keine pauschale Widerrufsbelehrung für alle Geschäftsmodelle ausgeben.

---

# 54. BFSG / Accessibility Hinweis

Wenn BFSG einschlägig und eine gesetzlich erforderliche Information zur Barrierefreiheit notwendig ist, diese in die richtige Stelle integrieren.

Keine erfundene Konformitätserklärung.

Keine Behauptung:

> „WCAG AAA zertifiziert"

ohne tatsächliche Prüfung und Nachweis.

---

# 55. DSGVO vs. TDDDG sauber trennen

Claude muss unterscheiden:

- **TDDDG § 25**: Zugriff/Speicherung auf der Endeinrichtung
- **DSGVO**: Verarbeitung personenbezogener Daten

Je nach Technologie können **beide** Ebenen relevant sein.

Nicht sagen:

> „Cookie-Banner = DSGVO und damit alles erledigt."

Ein Consent-Tool ersetzt nicht die Datenschutzerklärung, Verträge oder korrekte technische Implementierung.

---

# 56. Consent technisch testen

Bei aktivierungspflichtigen Diensten:

### Vor Zustimmung

- keine entsprechenden Requests
- keine entsprechenden Cookies/Storage-Werte
- keine Analytics-/Marketing-Skripte
- keine eingebettete Drittanbieterkommunikation, soweit diese gerade dadurch ausgelöst würde

### Nach Zustimmung

- Dienst lädt korrekt
- Einwilligung wird gespeichert
- Zweck korrekt dokumentiert

### Nach Widerruf

- weitere Nutzung blockieren, soweit technisch möglich/erforderlich
- Consent-Status aktualisieren
- weitere Verarbeitung beenden, soweit erforderlich

---

# 57. Browser-/Netzwerkprüfung

Vor Release DevTools öffnen:

- Network
- Application/Storage
- Cookies
- Local Storage
- Session Storage
- Console

Suche nach:

- `google-analytics`
- `googletagmanager`
- `facebook`
- `connect.facebook`
- `doubleclick`
- `youtube`
- `maps.googleapis`
- externe Fonts
- unbekannte Domains

Jede gefundene Domain muss erklärt werden können.

---

# 58. Abhängigkeiten

Vor Deployment:

- `npm audit` bzw. entsprechendes Tool
- veraltete Libraries prüfen
- bekannte CVEs prüfen
- ungenutzte Packages entfernen
- Lockfile committed
- Build reproduzierbar halten

Keine unsicheren Paketversionen ohne bewusst dokumentierte Ausnahme.

---

# 59. Frontend-Code-Regeln

Bevorzugen:

- semantisches HTML
- progressive enhancement
- kleine Abhängigkeiten
- keine unnötigen Frameworks
- keine Inline-Secrets
- keine unnötigen externen Skripte
- CSP-kompatibler Aufbau
- sichere DOM-APIs

---

# 60. JavaScript-Sicherheit

Vorsicht bei:

- `innerHTML`
- `outerHTML`
- `document.write`
- `eval`
- dynamischem Script-Laden
- unsicheren URL-Parametern

Nutzereingaben niemals ungeprüft als HTML ausgeben.

---

# 61. SEO ohne rechtliches Risiko

SEO-Optimierung darf nicht zu irreführenden Aussagen führen.

Prüfen:

- Title
- Meta Description
- Canonical
- Sitemap
- robots.txt
- strukturierte Daten
- Open Graph
- Twitter/X Cards

Keine erfundenen:

- Bewertungen
- Preise
- Produktverfügbarkeiten
- Aggregate Ratings
- Auszeichnungen

---

# 62. Strukturierte Daten

Nur strukturierte Daten ausgeben, die den sichtbaren und tatsächlichen Inhalt widerspiegeln.

Keine Fake-Reviews oder erfundene Aggregate Ratings.

---

# 63. Accessibility + SEO gemeinsam

Semantische Struktur nutzen:

- genau ein sinnvoller Haupttitel
- logisch verschachtelte Überschriften
- beschreibende Linktexte
- `lang="de"`
- Landmarken
- Alternativtexte

Beispiel:

```html
<html lang="de">
```

Nicht:

```html
<a href="/kontakt">Hier klicken</a>
```

besser:

```html
<a href="/kontakt">Kontakt aufnehmen</a>
```

---

# 64. Meta-Informationen

Keine personenbezogenen Daten in:

- Title
- URLs
- Meta Description
- Open-Graph-Tags
- strukturierte Daten

ohne sachlichen Grund.

---

# 65. Kontaktinformationen

Firmenkontakt klar darstellen:

- Firma
- Adresse
- E-Mail
- ggf. Telefon
- ggf. Geschäftszeiten

Telefonnummer ist nicht zwingend immer gesetzlich auf jeder einfachen Website vorgeschrieben; bei gesetzlichen Pflichtangaben immer den konkreten Fall prüfen.

---

# 66. Datenschutz-Link

Footer:

```html
<a href="/datenschutz">Datenschutz</a>
<a href="/impressum">Impressum</a>
```

Bei Consent-Systemen zusätzlich beispielsweise:

```html
<button type="button" data-open-consent-settings>
  Cookie-Einstellungen
</button>
```

---

# 67. Rechtstexte nicht hardcoden, wenn CMS genutzt wird

Bei größeren Websites sollen Rechtstexte einfach aktualisierbar sein.

Struktur:

```text
/content
  /legal
    impressum
    datenschutz
    accessibility
```

Bei statischen Sites sauber zentral verwalten.

---

# 68. Versionierung der Rechtstexte

Intern dokumentieren:

- Version
- Datum
- verantwortliche Person
- Anlass der Änderung
- betroffene Dienste

Nicht notwendigerweise öffentlich als technische Versionsnummer anzeigen, aber intern nachvollziehbar halten.

---

# 69. Legal Change Detection

Bei Änderungen an:

- Analytics
- Fonts
- Hosting
- Formular
- CRM
- Newsletter
- Maps
- Videos
- Chat
- Social Media
- Payment
- Login

muss eine erneute Datenschutz-/Rechtsprüfung ausgelöst werden.

---

# 70. Content Governance

Vor Veröffentlichung:

- Firmennamen korrekt
- Anschrift korrekt
- Kontakt korrekt
- Leistungsversprechen wahr
- Preise korrekt
- Referenzen echt
- Kundenlogos erlaubt
- Teamangaben korrekt
- Zertifikate aktuell
- Jahreszahlen aktuell

---

# 71. Abmahnrisiko reduzieren

Besonders sorgfältig prüfen:

- Impressum
- Datenschutz
- Preisangaben
- Werbeclaims
- Urheberrechte
- Marken
- Bilder
- Kundenlogos
- Cookie/Tracking
- Formulierungen zu Garantien
- Aussagen über Wettbewerber
- Fake-Bewertungen

---

# 72. Rechtstext-Platzhalter

Wenn Unternehmensdaten fehlen, verwende beispielsweise:

```text
[FIRMENNAME]
[RECHTSFORM]
[GESCHÄFTSFÜHRUNG]
[ANSCHRIFT]
[PLZ ORT]
[EMAIL]
[TELEFON]
[HANDELSREGISTERNUMMER]
[REGISTGERICHT]
[UST-ID]
[WIRTSCHAFTS-ID]
[AUFSICHTSBEHÖRDE]
[BERUFSKAMMER]
[BERUFSBEZEICHNUNG]
[BERUFSRECHTLICHE REGELUNGEN]
[DATENSCHUTZKONTAKT]
```

Nie ausdenken.

---

# 73. Projekt-Matrix für die erste Analyse

Vor dem Coding eine Matrix erstellen:

| Feature | Vorhanden? | personenbezogene Daten? | Drittanbieter? | Consent? | Rechtstext? | Barrierefreiheit? | Test |
|---|---|---|---|---|---|---|---|
| Kontaktformular | | | | | | | |
| Google Maps | | | | | | | |
| YouTube | | | | | | | |
| Analytics | | | | | | | |
| Newsletter | | | | | | | |
| Blog | | | | | | | |
| Terminbuchung | | | | | | | |
| Login | | | | | | | |

---

# 74. Minimaler Firmenwebsite-Footer

Beispielstruktur:

```html
<footer>
  <nav aria-label="Rechtliche Informationen">
    <a href="/impressum">Impressum</a>
    <a href="/datenschutz">Datenschutz</a>
  </nav>
</footer>
```

Weitere Links nur hinzufügen, wenn sie tatsächlich benötigt werden, z. B.:

- Barrierefreiheit
- Cookie-Einstellungen
- AGB
- Widerruf
- Kündigung
- Versand
- Zahlungsinformationen

---

# 75. Keine unnötigen Rechtstexte

Nicht jede Firmenwebsite braucht:

- AGB
- Widerrufsbelehrung
- Widerrufsformular
- Versandbedingungen
- Kündigungsbutton
- Shop-Hinweise

Diese nur verwenden, wenn das Geschäftsmodell das erfordert.

---

# 76. Keine falsche Rechtsberatung

Wenn ein Nutzer fragt:

> „Ist das garantiert legal?“

antworten:

> „Nach dem derzeit geprüften Stand und unter den genannten Annahmen entspricht die Umsetzung den identifizierten Anforderungen. Eine individuelle rechtliche Beratung oder Freigabe ersetzt diese Prüfung nicht. Bei Zweifelsfällen sollte ein deutscher Rechtsanwalt bzw. Datenschutzexperte die konkrete Website prüfen."

---

# 77. Deep Research Trigger

Wenn eine konkrete Rechtsfrage nicht sicher aus dem vorhandenen Wissen beantwortet werden kann:

1. offizielle Primärquelle suchen
2. aktuelle Fassung prüfen
3. Anwendungsbereich prüfen
4. nur belastbare Schlussfolgerung ziehen
5. Quelle im Ergebnis nennen

Bei zeitabhängigen Themen immer aktuelles Datum beachten.

---

# 78. Launch-Gate

Eine Website gilt intern erst dann als „bereit“, wenn alle folgenden Gate-Kategorien auf PASS stehen:

```text
LEGAL
[ ] Impressum geprüft
[ ] Datenschutz geprüft
[ ] Cookies/TDDDG geprüft
[ ] Tracking geprüft
[ ] Urheberrechte geprüft
[ ] Bildrechte geprüft
[ ] Marken geprüft
[ ] Werbeaussagen geprüft
[ ] branchenspezifische Pflichten geprüft

ACCESSIBILITY
[ ] Tastatur
[ ] Fokus
[ ] Screenreader-Basis
[ ] Alt-Texte
[ ] Kontrast
[ ] Formulare
[ ] mobile Darstellung
[ ] semantisches HTML
[ ] BFSG-Anwendbarkeit geprüft

SECURITY
[ ] HTTPS
[ ] Secrets entfernt
[ ] XSS geprüft
[ ] CSRF geprüft
[ ] Injection geprüft
[ ] Headers geprüft
[ ] Dependencies geprüft
[ ] Backups
[ ] Admin geschützt

PRIVACY
[ ] Dateninventar
[ ] Drittanbieterinventar
[ ] Consent getestet
[ ] Widerruf getestet
[ ] Datenschutzerklärung stimmt mit Code überein
[ ] AV-Verträge geprüft, soweit relevant
[ ] Löschkonzept

CONTENT
[ ] Firmendaten korrekt
[ ] Texte korrekt
[ ] Preise korrekt
[ ] Referenzen echt
[ ] Bildlizenzen dokumentiert
[ ] Marken-/Logo-Nutzung erlaubt

FUNCTIONAL
[ ] Navigation
[ ] Formulare
[ ] Fehlermeldungen
[ ] 404
[ ] mobile
[ ] Desktop
[ ] Performance
[ ] SEO-Basis
```

---

# 79. Release-Ablauf

Claude soll grundsätzlich in dieser Reihenfolge arbeiten:

### Phase A — Anforderungen

1. Geschäftsmodell identifizieren.
2. Zielgruppe identifizieren.
3. Firmenstandort/Rechtsform erfassen.
4. Online-Vertragsabschluss feststellen.
5. Externe Dienste erfassen.
6. Datenflüsse erfassen.
7. BFSG-Anwendbarkeit prüfen.
8. branchenspezifische Gesetze prüfen.

### Phase B — Architektur

1. Seitenstruktur
2. semantisches HTML
3. Datenschutzarchitektur
4. Consent-Architektur
5. Sicherheitsarchitektur
6. Accessibility
7. Performance

### Phase C — Implementierung

1. HTML
2. CSS
3. JS
4. serverseitige Funktionen
5. Consent
6. Formulare
7. Rechtstexte

### Phase D — Test

1. Browser
2. Mobile
3. Keyboard
4. Screenreader-Basis
5. Network/Storage
6. Security
7. Privacy
8. Content

### Phase E — Launch

Nur veröffentlichen, wenn keine offene rote/blockierende Anforderung vorhanden ist.

---

# 80. Definition of Done

Die Firmenwebsite ist „Done“, wenn:

- reale Firmendaten eingesetzt sind
- Impressum korrekt ist
- Datenschutzerklärung zur tatsächlichen Implementierung passt
- TDDDG-/Consent-Themen geprüft sind
- alle externen Dienste inventarisiert sind
- nicht notwendiges Tracking erst nach Einwilligung startet
- Bild-/Text-/Asset-Rechte geklärt sind
- Barrierefreiheit technisch geprüft ist
- BFSG-Anwendbarkeit beurteilt ist
- HTTPS aktiv ist
- Sicherheits-Basismaßnahmen umgesetzt sind
- Formulare sicher funktionieren
- keine Secrets im Frontend liegen
- Rechtstexte erreichbar sind
- wesentliche Aussagen wahr und belegbar sind
- alle Tests bestanden sind
- offene Rechtsfragen klar markiert und ggf. zur Fachprüfung eskaliert wurden

---

# 81. Harte Verbote

Claude darf bei einer deutschen Firmenwebsite niemals:

- Unternehmensdaten erfinden
- fake Zertifikate erfinden
- fake Kunden erfinden
- fake Testimonials erfinden
- fake Bewertungen erzeugen
- fremde Bilder ohne geklärte Lizenz einbauen
- fremde Texte kopieren
- Tracking heimlich aktivieren
- notwendige Consent-Prüfungen umgehen
- API-Secrets in clientseitigen Code schreiben
- Passwörter im Klartext speichern
- „rechtssicher garantiert“ behaupten
- ein generisches Impressum als endgültig korrekt darstellen
- eine generische Datenschutzerklärung als passend behaupten, ohne die Website zu analysieren
- BFSG-Konformität behaupten, ohne entsprechende Prüfung
- WCAG-Konformität auf einer bloßen Behauptung aufbauen

---

# 82. Technische Qualitätsregeln

Code soll:

- wartbar
- modular
- verständlich
- performant
- sicher
- semantisch
- zugänglich
- möglichst dependency-arm

sein.

Keine unnötigen Libraries nur für kleine Funktionen.

---

# 83. Empfehlung für eine einfache Firmenwebsite

Für eine normale Unternehmensseite ohne Shop und ohne Login ist folgende Architektur besonders robust:

```text
Home
Leistungen
Über uns
Referenzen
Kontakt
Impressum
Datenschutz

+ Cookie-Einstellungen nur wenn tatsächlich benötigt
+ Barrierefreiheit-Information nur wenn erforderlich/angezeigt sinnvoll
```

Technisch möglichst:

- statisches HTML/CSS/JS
- selbst gehostete Fonts
- keine unnötigen Third-Party-Skripte
- serverseitiges Kontaktformular oder datenschutzbewusster Dienst
- HTTPS
- minimaler JavaScript-Fußabdruck

---

# 84. Finaler Claude-Output bei Website-Erstellung

Nach Fertigstellung muss Claude eine kurze Compliance-Zusammenfassung liefern:

```text
LEGAL CHECK
Status: PASS / PARTIAL / BLOCKED

Impressum: PASS/PARTIAL/BLOCKED
Datenschutz: PASS/PARTIAL/BLOCKED
TDDDG/Consent: PASS/PARTIAL/BLOCKED
Externe Dienste: PASS/PARTIAL/BLOCKED
Urheber-/Bildrechte: PASS/PARTIAL/BLOCKED
Barrierefreiheit: PASS/PARTIAL/BLOCKED
Security: PASS/PARTIAL/BLOCKED
Branchenspezifische Regeln: PASS/PARTIAL/BLOCKED

OFFENE PUNKTE
- ...

RECHTLICHE PRÜFUNG ERFORDERLICH
- ...
```

Wenn `BLOCKED` vorliegt, darf Claude die Website nicht als vollständig launchbereit bezeichnen.

---

# 85. Quellenprinzip

Bei konkreten gesetzlichen Aussagen nach Möglichkeit die Primärquelle verwenden.

Besonders wichtige Referenzpunkte:

- DDG § 5: Anbieterinformationen
- TDDDG § 25: Zugriff/Speicherung auf Endeinrichtungen
- BFSG § 3: Anwendungsbereich/Ausnahme für Kleinstunternehmen bei Dienstleistungen
- BFSGV § 19: Anforderungen an Dienstleistungen im elektronischen Geschäftsverkehr
- BGB § 312j: besondere Pflichten im elektronischen Geschäftsverkehr
- BGB § 355: Widerrufsrecht
- PAngV § 3: Gesamtpreis
- PAngV § 11: niedrigster Preis der letzten 30 Tage bei Preisermäßigungen
- UWG §§ 5, 7: Irreführung und Werbung/elektronische Post, soweit anwendbar
- UrhG § 19a: öffentliche Zugänglichmachung
- KunstUrhG § 22: Bildnisse

Diese Liste ist nicht abschließend. Immer den konkreten Sachverhalt prüfen.

---

# 86. Verhalten bei fehlenden Informationen

Wenn für eine rechtliche oder technische Entscheidung Informationen fehlen, darf Claude nicht raten.

Stattdessen:

1. Website best-effort weiterbauen.
2. fehlende Information als `[OFFEN: ...]` markieren.
3. konkrete Auswirkung beschreiben.
4. relevante Rechtsnorm/technischen Bereich nennen.
5. nach Möglichkeit eine sichere Default-Option wählen.

Beispiel:

```text
[OFFEN: Wird Google Analytics tatsächlich benötigt?]
Auswirkung: Consent-/Datenschutzarchitektur und Drittlandprüfung ändern sich.
Sichere Default-Option: Analytics deaktiviert lassen.
```

---

# 87. Wichtigste Leitlinie

**Die Website bestimmt die Rechtstexte – nicht umgekehrt.**

Erst tatsächliche Funktionen und Datenflüsse ermitteln.
Dann Rechtsgrundlagen und Pflichten bestimmen.
Dann Technik und Rechtstexte synchron umsetzen.
Danach testen.
Dann veröffentlichen.

Nicht:

> „Wir haben eine Datenschutzerklärung, also ist die Website DSGVO-konform."

Sondern:

> „Der tatsächliche Datenfluss wurde analysiert, technisch minimiert, rechtlich eingeordnet, dokumentiert und mit den veröffentlichten Informationen abgeglichen."

---

# Ende
