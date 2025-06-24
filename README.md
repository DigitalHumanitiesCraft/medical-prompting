# Medical Prompting Quickstart-Guide

Bei medizinischen Fragen führen direkte Anfragen an LLMs oft zu oberflächlichen oder ungenauen Antworten. Dieser Guide zeigt Ihnen, wie Sie durch strategisches Prompting verlässliche, gut durchdachte medizinische Informationen erhalten.

## Grundprinzip: Kontext aufbauen, dann validieren

LLMs funktionieren am besten, wenn Sie sie durch logische Schritte führen, anstatt sofortige Schlussfolgerungen zu verlangen. Denken Sie daran, als würden Sie der KI beibringen, ihre "Arbeit zu zeigen."

## Strategie 1: Mehrstufiges kontextuelles Prompting

**❌ Machen Sie das nicht:**
> "Ich habe einen Bandscheibenvorfall in der Halswirbelsäule. Welche Übungen soll ich machen?"

**✅ Machen Sie stattdessen das:**

1. **Fundament legen:**
   ```
   Ich habe einen Bandscheibenvorfall bei C5-C6. Welche spezifischen Muskelgruppen sind von diesem Zustand am meisten betroffen?
   ```

2. **Kontext aufbauen:**
   ```
   Für die Muskelgruppen, die du erwähnt hast, welche Arten von Übungen werden allgemein für Kräftigung und Flexibilität empfohlen?
   ```

3. **Spezifisch werden:**
   ```
   Basierend auf diesen Informationen, erstelle ein anfängerfreundliches Übungsprogramm für jemanden mit einem C5-C6 Bandscheibenvorfall.
   ```

4. **Validierung erzwingen (LLM-Poking):**
   ```
   Überprüfe diesen Übungsplan nochmal kritisch. Ist das wirklich angemessen und sicher? Liste mögliche Bedenken oder nötige Anpassungen auf und erkläre deine Begründung.
   ```

### Warum das funktioniert
- Jeder Schritt baut logischen Kontext auf
- Das LLM kann wichtige Überlegungen nicht überspringen
- Abschließende Validierung fängt Versäumnisse oder unsichere Empfehlungen ab

## Strategie 2: Pseudo-Präzision mit aggressiver Faktenprüfung bekämpfen

LLMs hassen es, "Ich weiß es nicht" zu sagen und liefern oft selbstsicher klingende, aber ungenaue Zahlen oder Fakten.

**❌ Gefährliche Frage:**
> "Wie lange bleiben die Antioxidantien in grünem Tee nach dem Aufbrühen stabil?"

**✅ Besserer Ansatz:**

1. **Mit eingebauter Unsicherheit fragen:**
   ```
   Was sagt die aktuelle Forschung über die Stabilität von Antioxidantien in aufgebrühtem grünem Tee im Zeitverlauf? Sei spezifisch darüber, was du weißt vs. was unsicher ist.
   ```

2. **Ehrlichkeit erzwingen:**
   ```
   Sei absolut ehrlich bei Fakten und Zahlen, die du nicht genau weißt. Nutze Webrecherche für Behauptungen, bei denen du unsicher bist, und wenn du keine 100% bewiesenen Fakten findest, sag das explizit.
   ```

3. **Quellen validieren:**
   ```
   Welche spezifischen Studien oder Quellen unterstützen diese Zeiträume? Wenn du Schätzungen machst, kennzeichne sie klar als solche.
   ```

## Schnellreferenz: Validierungsphrasen für Prompts

Verwenden Sie diese "LLM-Poking" Formulierungen in Ihren Prompts:

- `"Ist das wirklich genau? Überprüfe deine Begründung nochmal."`
- `"Bei was bist du in dieser Antwort unsicher?"`
- `"Liste potenzielle Risiken oder Kontraindikationen auf, die ich wissen sollte."`
- `"Sei völlig ehrlich darüber, was die aktuelle Forschung unterstützt vs. nicht unterstützt."`
- `"Suche nach aktuellen Studien, um diese Behauptungen zu verifizieren."`
- `"Wenn du dir nicht sicher bist, sag es direkt."`
- `"Erkläre, woher du diese Zahlen hast."`

## Die goldene Regel

**Akzeptieren Sie niemals die erste Antwort bei medizinischen Fragen.** Iterieren Sie immer mindestens 2-3 Mal mit Validierungsprompts. Die zweite und dritte Antwort des LLMs ist typischerweise viel genauer und nuancierter.

## Warnsignale, auf die Sie achten sollten

- Übermäßig selbstsichere Antworten auf komplexe Fragen
- Spezifische Zahlen ohne zitierte Quellen
- Allgemeine Ratschläge, die individuelle Unterschiede nicht berücksichtigen
- Antworten, die nicht erwähnen, Gesundheitsfachkräfte zu konsultieren

---

> Für Workshos zum Thema Generative KI und Prompt Engineering kontaktieren Sie uns gerne: office@dhcraft.org
