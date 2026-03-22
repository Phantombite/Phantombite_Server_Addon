# DEV Funktion — PhantomBite Server Addon

## Zweck
Serverseitige Anpassungen von Vanilla-Blöcken und Spielmechaniken speziell für den Dune/Nimbus Server. Keine eigenen Blöcke — nur Wert-Änderungen an bestehenden Vanilla-Definitionen.

## Inhalt

### CubeBlocks_Energy.sbc — Energie-Blöcke
Angepasste Wasserstoffmotoren und Wasserstofftanks:
- Wasserstoffmotoren (Large/Small, Normal/Reskin): MaxPowerOutput 5 MW / 0.5 MW
- Wasserstofftanks (alle Varianten inkl. Industrial)

### CubeBlocks_Logistics.sbc — Logistik-Blöcke
Angepasste Logistik-Blöcke für den Server.

### CubeBlocks_OreDetectors.sbc — Erzdetektoren
- Large Grid OreDetector: Reichweite 450m
- Small Grid OreDetector: Reichweite 150m
- Reskin Varianten: gleiche Reichweiten

### CubeBlocks_Thrusters.sbc — Triebwerke
Angepasste Wasserstofftriebwerke (Normal + Industrial + Reskin Varianten).

### Blueprints_RadiationKit.sbc — Radiation Kit Rezept
SE hat kein Vanilla-Rezept für das Radiation Kit — dieses Blueprint fügt es hinzu.

**Rezept:**
- 1x Medkit
- 2x Medical Component
- 5x Mushrooms
- 0.5x Uranium Ingot

**Verfügbar in:** EliteEquipment, SimpleEquipment Assembler-Klassen

### Fraktionsschutz/Reputation.sbc — Fraktionsruf
Verhindert Ruf-Verlust bei allen Aktionen:

| Aktion | Ruf-Verlust |
|--------|-------------|
| Schaden | 0 |
| Schleifen/Schweißen | 0 |
| Angreifen | 0 |
| Stehlen | 0 |
| Töten | 0 |
| Piraten (alle) | 0 |

Maximaler Rufgewinn pro Zeiteinheit: 100 (alle 30 Minuten zurückgesetzt).

## Abhängigkeiten
Keine — dieser Mod hat keine Abhängigkeiten.

## Dateistruktur
```
Phantombite_Server_Addon/
├── modinfo.sbmi
├── metadata.mod
└── Data/
    ├── Blueprints/Blueprints_RadiationKit.sbc
    ├── CubeBlocks/
    │   ├── CubeBlocks_Energy.sbc
    │   ├── CubeBlocks_Logistics.sbc
    │   ├── CubeBlocks_OreDetectors.sbc
    │   └── CubeBlocks_Thrusters.sbc
    └── Fraktionsschutz/Reputation.sbc
```
