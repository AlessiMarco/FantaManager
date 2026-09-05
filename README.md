# FantaManager

Foglio d'asta per il fantacalcio in un unico file HTML, senza server e senza dipendenze.

- **Strategia e live** per ogni reparto (POR, DIF, CEN, ATT), con residuo, offerta massima e delta.
- **Vista telefono** dedicata sotto i 720 px: intestazione fissa con la strategia in vista, residuo, offerta massima e slot; un reparto alla volta.
- **Salvataggi** con nome e data. Di base vivono nel browser; collegando GitHub dal pannello Salvataggi diventano file JSON in questo stesso repo (`salvataggi/<id>.json`, più `corrente.json` per lo stato sincronizzato), uguali su PC e telefono e con la storia delle versioni. Esporta e importa in JSON restano come rete di sicurezza.

Il sito è pubblicato con GitHub Pages: apri il link in Safari e usa "Aggiungi alla schermata Home" per averlo come app.

Senza GitHub collegato i dati vivono solo nel browser che usi. Con GitHub collegato l'app parla direttamente con l'API di GitHub usando un token fine-grained limitato a questo repo, che resta salvato solo nel browser del dispositivo. Il repo è pubblico, quindi anche i salvataggi lo sono: contengono solo crediti per slot, nessun nome.
