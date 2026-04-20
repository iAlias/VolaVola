# VolaVola ✈️

**VolaVola** è un tracker di voli in tempo reale interamente client-side, costruito con HTML, CSS e JavaScript vanilla. Visualizza il traffico aereo su una mappa interattiva usando i dati dell'[OpenSky Network](https://opensky-network.org/).

---

## 🚀 Funzionalità

- 🗺️ **Mappa interattiva** (Leaflet.js) con tile dark/light personalizzabili
- 📡 **Dati in tempo reale** dall'API OpenSky Network, aggiornati ogni 10 secondi
- 🎯 **Modalità Demo** automatica: se l'API non è raggiungibile, vengono mostrati dati simulati realistici senza interrompere l'esperienza
- 🔍 **Ricerca** per callsign, numero volo o paese
- 🎚️ **Filtri** per altitudine, stato (in volo / a terra), paese di origine
- 📍 **Geolocalizzazione**: centra la mappa sulla posizione dell'utente e mostra i voli nelle vicinanze (entro 100 km)
- ✈️ **Dettagli volo**: callsign, altitudine, velocità, direzione, paese di origine
- 🛤️ **Traccia rotta**: percorso storico del volo selezionato
- 🌗 **Tema chiaro/scuro** con toggle in header
- 📱 **Responsive**: ottimizzato per mobile e desktop

---

## 🛠️ Tecnologie

| Tecnologia | Utilizzo |
|---|---|
| HTML / CSS / JS vanilla | Struttura, stile, logica |
| [Leaflet.js](https://leafletjs.com/) | Mappa interattiva |
| [OpenSky Network API](https://opensky-network.org/apidoc/) | Dati voli in tempo reale |
| [CartoDB](https://carto.com/) | Tile mappa (dark/light) |
| [Google Fonts](https://fonts.google.com/) | Inter + JetBrains Mono |

---

## 📂 Struttura del progetto

```
VolaVola/
└── flight-tracker/
    └── flight-tracker.html   # App completa, single-file
```

---

## ▶️ Come usarlo

1. Clona il repository:
   ```bash
   git clone https://github.com/iAlias/VolaVola.git
   ```
2. Apri `flight-tracker/flight-tracker.html` direttamente nel browser.

> **Nota:** l'app è interamente client-side e non richiede alcun backend o build step.

---

## ⚠️ Nota sull'API

L'API OpenSky Network è pubblica e gratuita, ma soggetta a limiti di rate e occasionali periodi di indisponibilità. Quando l'API non è raggiungibile (ad es. per limitazioni CORS del browser o downtime), l'app entra automaticamente in **Modalità Demo**: vengono mostrati 60 voli simulati sull'area italiana per permettere comunque di esplorare l'interfaccia.

---

## 📄 Licenza

Distribuito sotto licenza [MIT](LICENSE).
