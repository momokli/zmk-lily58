# Lily58 QWERTZ Gaming Layout 🎮

Für meinen Bruder. Linke Hälfte, QWERTZ, gaming — mehr braucht's nicht.

## Das Layout

### Normal (Default) — Tippen & Chatten

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
          │ ALT  │FUNK1 │LEERTAST│FUNK2│
          └──────┴──────┴──────┴──────┘
```

Das ist ein ganz normaler QWERTZ-Linksteil. WASD und alle wichtigen Tasten sind da, wo du sie kennst. Die Daumen bedienen ALT, LEERTASTE und die zwei Funktionstasten.

### Funktion 1 (FUNK1 gedrückt halten) — F-Tasten & Media

```
┌──────┬─────┬─────┬─────┬─────┬─────┬──────┐
│  F1  │ F2  │ F3  │ F4  │ F5  │ F6  │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│  F7  │ F8  │ F9  │ F10 │ F11 │ F12 │      │
├──────┼─────┼─────┼─────┼─────┼─────┤      │
│ LEISER│LAUTER│STUMM│PLAY │VORHER│NÄCHSTER│
├──────┼─────┼─────┼─────┼─────┼─────┼──────┤
│ ▶ Alles durchgereicht — Y, X, C, V, B usw. │
└──────┴─────┴─────┴─────┴─────┴─────┴──────┘
```

Ideal zum Zocken: F1-F12 für Ingame-Menüs, Lautstärke und Media-Tasten für Discord/Musik. Die untere Reihe und Daumen arbeiten normal weiter.

### Funktion 2 (FUNK2 gedrückt halten) — Z, Pfeiltasten & Sonderzeichen

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

- **Z** — zum Hinlegen/Kriechen (in QWERTZ ist Z auf der rechten Seite, hier haste sie trotzdem)
- **Pfeiltasten** — navigieren ohne rechte Hand
- **Sonderzeichen** — [], =, \, -
- **WIN-Taste** — für Gamebar (Win+G) usw.

## Wie benutzen?

1. **Linke Seite** anschließen, die rechte wird erstmal nicht gebraucht
2. Beim ersten Mal per USB anschließen, dann verbindet er sich automatisch
3. **FUNK1** = die zweite Taste von links unten (gedrückt halten = F-Tasten/Layer)
4. **FUNK2** = die vierte Taste von links unten (gedrückt halten = Z/Pfeile/Layer)
5. Loslegen — die wichtigsten Tasten sind genau wie auf ner normalen Tastatur

## QWERTZ-Hinweis

Die Tastatur sendet die Tasten auf Englisch (HID-Codes). Dein Betriebssystem muss auf **Deutsch (QWERTZ)** eingestellt sein, dann kommen die richtigen Buchstaben an. Besonders bei Y und Z: auf der Tastatur ist das Y physikalisch da wo früher Z war — das gehört so.

## Bauen & Flashen

```bash
# Firmware bauen (GitHub Actions macht das automatisch)
# Oder lokal:
west build -d build/left -b nice_nano_v2 -- -DSHIELD=splitkb_aurora_lily58_left
# Flashen:
west flash -d build/left
```

Die fertige Firmware liegt nach dem Build in GitHub Actions als Download bereit.

---

Viel Spaß beim Zocken! Bei Fragen oder Änderungswünschen einfach Bescheid sagen.
