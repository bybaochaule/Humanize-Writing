# Humanize Writing

Ein deutschsprachiger ChatGPT-Skill, der steif oder KI-typisch klingende Texte in natürliche, glaubwürdige Sprache verwandelt – ohne Fakten, Aussage oder persönliche Stimme zu verfälschen.

## Was dieser Skill macht

`humanize-writing` überarbeitet nicht nur einzelne Wörter. Der Skill erkennt typische KI-Muster, verbessert Aufbau und Rhythmus und passt den Text an Sprache, Zielgruppe und Medium an.

- Entfernt typische KI-Floskeln und unnötige Wiederholungen
- Verbessert Rhythmus, Satzlänge, Lesefluss und Struktur
- Bewahrt Fakten, Namen, Zahlen, Links und Fachbegriffe
- Erhält den gewünschten Stil: locker, formell, persönlich oder lokal
- Unterstützt deutsche, englische, vietnamesische und gemischtsprachige Texte
- Lokalisiert Redewendungen, Zeichensetzung, Datumsformate und Ton
- Verhindert, dass natürliche Texte zu glatter Werbe- oder Essaysprache werden

## Geeignet für

- E-Mails und Nachrichten
- Social-Media-Posts und Captions
- Blogartikel und Essays
- Produkt- und Werbetexte
- Bewerbungen und persönliche Texte
- Übersetzte oder mehrsprachige Inhalte
- Texte, die weniger nach ChatGPT oder KI klingen sollen

## Beispielanfragen

```text
Nutze @humanize-writing und schreibe diesen Text natürlicher, ohne die Bedeutung zu verändern.
```

```text
Entferne den KI-Geruch aus diesem Blogartikel. Der Ton soll freundlich und professionell bleiben.
```

```text
Schreibe diese Caption in natürlichem Vietnamesisch um. Behalte den persönlichen und humorvollen Ton.
```

```text
Humanisiere diese formelle E-Mail für eine deutschsprachige Geschäftskundin.
```

## Funktionsweise

Der Skill bewertet zunächst, wie stark ein Text nach KI klingt. Danach entscheidet er, ob eine kleine sprachliche Korrektur genügt oder der Text strukturell neu aufgebaut werden muss.

| Bewertung | Bedeutung | Vorgehen |
| --- | --- | --- |
| 0 | Bereits natürlich | Nur bei Bedarf minimal korrigieren |
| 1 | Kleine Auffälligkeiten | Leichte sprachliche Bereinigung |
| 2 | Einige KI-Spuren | Rhythmus und Übergänge verbessern |
| 3 | Deutlich künstlich | Struktur und Formulierungen überarbeiten |
| 4 | Stark mechanisch | Anhand der Kernaussagen neu schreiben |
| 5 | Unbrauchbar in der aktuellen Form | Bedeutung erhalten und vollständig neu aufbauen |

## Repository-Struktur

```text
humanize-writing/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── thumbnail.png
└── references/
    └── rewrite-playbook.md
```

## Installation

1. Dieses Repository herunterladen oder klonen.
2. Den Ordner `humanize-writing` vollständig übernehmen.
3. Darauf achten, dass `SKILL.md`, `agents/` und `references/` gemeinsam im selben Skill-Ordner bleiben.
4. Den Skill mit einer Anfrage wie `Nutze @humanize-writing ...` aufrufen.

## Wichtige Grundsätze

- Bedeutung und überprüfbare Inhalte bleiben erhalten.
- Gemischtsprachige Texte werden nicht ungefragt vollständig übersetzt.
- Persönliche Eigenheiten, Humor und lokale Sprachfärbung dürfen bestehen bleiben.
- Der Text wird nicht künstlich lässig, werblich oder übermäßig perfekt gemacht.

## Enthaltene Dateien

- [`SKILL.md`](SKILL.md) – Kernanweisungen und Ausgaberegeln
- [`rewrite-playbook.md`](references/rewrite-playbook.md) – ausführlicher Arbeitsablauf, Sprachregeln und Vorher-nachher-Beispiele
- [`openai.yaml`](agents/openai.yaml) – Anzeigename, Kurzbeschreibung und Standardanfrage

## Hinweis zur Verwendung

Vor einer öffentlichen Veröffentlichung empfiehlt es sich, eine passende Lizenz für das Repository festzulegen. In diesem Paket ist bewusst noch keine Lizenz vorgegeben.
