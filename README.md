# Lily58 QWERTZ Gaming Layout 🎮

QWERTZ-Layout für die **linke Hälfte** der splitkb Aurora Lily58. Fokus auf Gaming, die rechte Seite wird (noch) nicht gebraucht.

## Layout

### Default — Tippen

```
┌──────┬─────┬─────┬─────┬─────┬─────┬──────┐
│ ESC  │  1  │  2  │  3  │  4  │  5  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│ TAB  │  Q  │  W  │  E  │  R  │  T  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│STRG  │  A  │  S  │  D  │  F  │  G  │      │
├──────┼─────┼─────┼─────┼─────┼─────┼──────┤
│SHIFT │  Y  │  X  │  C  │  V  │  B  │  `   │
└──────┴─────┴─────┴─────┴─────┴─────┴──────┘
          ┌──────┬──────┬──────┬──────┐
          │ ALT  │FUNK1 │SPACE │FUNK2│
          └──────┴──────┴──────┴──────┘
```

Standard QWERTZ-Linksteil. WASD, STRG, Shift, Leertaste — alles an gewohnter Position.

### FUNK1 (halten) — F-Tasten & Media

```
┌──────┬─────┬─────┬─────┬─────┬─────┬──────┐
│  F1  │ F2  │ F3  │ F4  │ F5  │ F6  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│  F7  │ F8  │ F9  │ F10 │ F11 │ F12 │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│ LEISER│LAUTER│STUMM│PLAY │VOR  │NÄCHST│    │
├──────┼─────┼─────┼─────┼─────┼─────┼──────┤
│ untere Reihe + Daumen arbeiten normal weiter │
└──────┴─────┴─────┴─────┴─────┴─────┴──────┘
```

F1-F12 für Ingame-Menüs, Media-Tasten für Discord/Spotify. Die untere Reihe (Y, X, C, V, B) bleibt unverändert.

### FUNK2 (halten) — Z, Pfeiltasten, Sonderzeichen

```
┌──────┬─────┬─────┬─────┬─────┬─────┬──────┐
│  `   │  1  │  2  │  3  │  4  │  5  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│ ESC  │  Z  │  W  │  E  │  R  │  T  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│ ←    │ ↓   │ ↑   │ →   │POS1 │ENDE │      │
├──────┼─────┼─────┼─────┼─────┼─────┼──────┤
│ WIN  │FESTST│  -  │  =  │  [  │  ]  │  \   │
└──────┴─────┴─────┴─────┴─────┴─────┴──────┘
```

- **Z** — in QWERTZ normal auf der rechten Seite, hier trotzdem erreichbar
- **Pfeiltasten** — Navigation ohne rechte Hand
- **Sonderzeichen** — [], =, \, -
- **WIN-Taste** — für Gamebar (Win+G) etc.
- Die Daumentasten arbeiten normal weiter

## Benutzung

1. **Nur die linke Hälfte** anschließen (per USB)
2. FUNK1 = zweite Taste von links unten (gedrückt halten aktiviert Layer 1)
3. FUNK2 = vierte Taste von links unten (gedrückt halten aktiviert Layer 2)
4. OS-Tastaturlayout auf **Deutsch (QWERTZ)** stellen

## QWERTZ-Hinweis

Die Tastatur sendet HID-Scancodes. Das Betriebssystem muss auf Deutsch (QWERTZ) eingestellt sein, damit die richtigen Buchstaben ankommen. Der Y/Z-Tausch ist korrekt abgebildet.

## Build

```bash
# GitHub Actions baut automatisch bei jedem Push
# Manuell:
west build -d build/left -b nice_nano_v2 -- -DSHIELD=splitkb_aurora_lily58_left
west flash -d build/left
```

Die fertige Firmware (.uf2) liegt in den GitHub Actions Artefakten.
