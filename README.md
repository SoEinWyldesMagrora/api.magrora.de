```md
# Unsere API

Mit unserer API erhältst du kostenlosen Zugriff auf zahlreiche Dienste, die normalerweise kostenpflichtig sind.

## Aktuell verfügbar:

Derzeit unterstützen wir alle OPSUCHT-APIs. Zudem haben wir ein umfassendes Statistiksystem entwickelt, mit dem du die Preisentwicklungen der vergangenen Wochen abrufen kannst. Darüber hinaus bieten wir weitere nützliche Server-Statistiken, wie die aktuelle Spieleranzahl, grundlegende Serverdaten und vieles mehr.

## Das Beste daran:

Unsere API kann völlig kostenlos in deine Projekte integriert und genutzt werden.

### Beispiel für eine API-Abfrage:

```json
{
  "server": "opsucht",
  "onlinePlayers": 1247,
  "maxPlayers": 5000,
  "lastWeekPrices": {
    "diamant": [12000, 12500, 11800, 13000, 12750, 12200, 11900],
    "gold": [7500, 7300, 7200, 7100, 7050, 6900, 6800]
  },
  "status": "online"
}
```

### So nutzt du unsere API:

Du kannst einfach eine GET-Anfrage an unsere API senden:

```bash
curl -X GET "https://api.magrora.de/item/DIRT"
```

Die Antwort enthält dann alle relevanten Informationen zum Server.

## Grundlagen der API-Nutzung

Unsere API ist einfach in bestehende Projekte integrierbar. Im Folgenden findest du einige grundlegende Konzepte und Code-Beispiele.

### Installation eines benötigten Pakets:

Falls du die API in einem Node.js-Projekt nutzen möchtest, installiere zuerst das benötigte Paket:

```bash
npm install axios
```

### Beispiel für eine API-Abfrage:

Mit JavaScript kannst du ganz einfach eine Anfrage an die API senden:

```javascript
const axios = require('axios');

axios.get('https://api.magrora.de/item/DIRT')
  .then(response => {
    console.log(response.data);
  })
  .catch(error => {
    console.error('Fehler bei der API-Anfrage:', error);
  });
```

### Code-Beispiele für HTML, CSS und JavaScript:

- **HTML5**:
```html
<div id="status">Lade Daten...</div>
```

- **CSS**:
```css
#status { color: green; font-weight: bold; }
```

- **JavaScript**:
```javascript
document.getElementById('status').innerText = 'Server Online';
```

## Schritt-für-Schritt-Anleitung zur API-Nutzung:

1. Erstelle ein Konto und erhalte einen API-Key.
2. Führe eine Anfrage an die API mit deinem Key aus.
3. Verarbeite die erhaltenen Daten in deinem Projekt.
4. Optimiere deine Abfragen für bessere Performance.

## Wichtige Hinweise zur API:

### Hinweis:
Stelle sicher, dass du den API-Key nicht öffentlich teilst, um Missbrauch zu vermeiden.

### Warnung:
Die API hat ein Ratenlimit. Zu viele Anfragen in kurzer Zeit können zu einer Sperrung führen.

### Tipp:
Nutze die Caching-Mechanismen deines Backends, um unnötige API-Anfragen zu vermeiden.

### Fehler:
Falls du einen Fehler 403 erhältst, könnte dein API-Key ungültig oder abgelaufen sein.

## API-Daten und -Technologien

In der API-Entwicklung sind strukturierte Daten und gut dokumentierte Endpunkte entscheidend. Hier zeigen wir, wie du wichtige Technologien und Tools nutzen kannst, um leistungsfähige APIs zu erstellen und zu integrieren.

### API-Status mit Lightbox:
Klicke auf das Bild, um eine detaillierte Ansicht des API-Status und Fehlercodes zu erhalten.

### API-Status Beispiel:

| Antwort-Code | Bedeutung                                   |
|--------------|---------------------------------------------|
| 200          | OK - Die Anfrage wurde erfolgreich verarbeitet. |
| 400          | Bad Request - Die Anfrage war fehlerhaft, z. B. fehlende Parameter. |
| 500          | Internal Server Error - Es gab einen Fehler auf der Serverseite. |

### Vergleich von API-Frameworks:

| Framework             | Beschreibung                                                        |
|-----------------------|---------------------------------------------------------------------|
| **Express.js**         | Ein minimalistisches Webframework für Node.js, das sich hervorragend für RESTful APIs eignet. |
| **Flask**              | Ein leichtgewichtiges Python-Framework, das sich ideal für die schnelle API-Entwicklung eignet. |
| **Django Rest Framework** | Ein robustes Framework für die Erstellung von RESTful APIs mit Django. |

### Top Technologien für API-Entwicklung:

| #  | Technologie | Hauptverwendung                               |
|----|-------------|-----------------------------------------------|
| 1  | REST        | Standard für Web-APIs, bei dem HTTP-Anfragen verwendet werden, um Ressourcen zu manipulieren. |
| 2  | GraphQL     | Eine flexible API-Technologie, die es ermöglicht, nur die benötigten Daten abzufragen. |
| 3  | WebSocket   | Für bidirektionale Echtzeitkommunikation in Webanwendungen. |

## Wie kann ich die API effektiv nutzen?

Die API ist darauf ausgelegt, einfache Integration und schnellen Zugriff auf Daten zu ermöglichen. Vergewissere dich, dass du die Rate Limits beachtest und deine Authentifizierung korrekt vornimmst. Achte auch darauf, die richtigen Endpunkte zu verwenden, um Fehler zu vermeiden.

## Was passiert, wenn ich einen Fehler erhalte?

Wenn du auf einen Fehler stößt, überprüfe zuerst die Fehlermeldung, die die API zurückgibt. In den meisten Fällen enthält die Fehlermeldung eine detaillierte Beschreibung des Problems und wie du es beheben kannst. Häufige Fehler sind ungültige Parameter oder überschrittene Rate Limits.

## Wann wird das Rate Limit zurückgesetzt?

Das Rate Limit wird einmal pro Stunde zurückgesetzt, basierend auf dem Unix-Zeitstempel, der in den Headern jeder Antwort enthalten ist. Stelle sicher, dass du das Limit nicht überschreitest, um eine Unterbrechung deines Zugriffs zu vermeiden.

## Wie kann ich den Support erreichen?

Wenn du Hilfe benötigst, wende dich bitte an unseren Support über das Kontaktformular auf unserer Website oder sende uns eine E-Mail an **info@magrora.de**. Wir sind immer bereit, dir zu helfen!

## Abschließende Worte

Wir danken dir, dass du unsere API verwendest! Wir hoffen, dass du mit den bereitgestellten Informationen gut zurechtkommst. Deine Fragen und Feedback helfen uns, die API kontinuierlich zu verbessern, sodass du das Beste aus ihr herausholen kannst.

**Viel Erfolg bei der Integration!**

Wir wünschen dir viel Erfolg bei der Nutzung unserer API und freuen uns darauf, dich bald wieder hier zu sehen. Bei weiteren Fragen stehen wir jederzeit zur Verfügung!
```
