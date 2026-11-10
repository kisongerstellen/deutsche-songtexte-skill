# Deutsche Songtexte – Skill für KI-Agenten

Ein deutschsprachiger Agent Skill für Claude Code und OpenAI Codex zum Schreiben und Überarbeiten von Songtexten.

Eine Idee, ein Gefühl oder eine Zeile, die dir nicht aus dem Kopf geht: Daraus kann ein Lied werden. Dieser Skill hilft dir, mit KI eigene deutsche Songtexte zu schreiben, passende Reime zu finden und einen Refrain zu entwickeln, der im Ohr bleibt.

Du hast schon einen Entwurf? Lass einzelne Zeilen überarbeiten, holprige Stellen glätten oder deinen Text an eine vorhandene Melodie anpassen.

Wenn du aus deinem fertigen Text einen [KI-Song erstellen](https://kisongerstellen.com/) möchtest, kannst du ihn bei KlangKI vertonen lassen. Auf [kisongerstellen.com](https://kisongerstellen.com/) entstehen aus eigenen Songtexten oder einer Beschreibung Songs mit Gesang und Instrumenten.

## Wobei dir der Skill hilft

- **Songtexte schreiben:** für Deutschpop, Schlager, Indie, Balladen, Rap oder ein persönliches Lied zum Geburtstag.
- **Refrains entwickeln:** die wichtigste Aussage auf wenige einprägsame Zeilen bringen.
- **Bessere Reime finden:** nach Klang auswählen, ohne dafür die Bedeutung oder den Satzbau zu verbiegen.
- **Texte überarbeiten:** deine Idee und deinen Ton erhalten, schwache Stellen gezielt verbessern.
- **Zu einer Melodie schreiben:** Silben, Betonungen und Atempausen an den vorhandenen Verlauf anpassen.
- **Ins Deutsche übertragen:** einen bereitgestellten Text so neu formulieren, dass er auf Deutsch natürlich klingt und singbar bleibt.

Der Skill achtet besonders auf das, was deutsche Songtexte schnell holprig macht: verdrehte Sätze, unnatürlich betonte Wörter, überladene Zeilen und Reime, die zwar klingen, aber nichts sagen.

## Songtexte mit Claude und Codex schreiben

Beschreibe, worum es gehen soll und wie der Text klingen darf. Wenn du schon Zeilen hast, füge sie hinzu und sage, was bleiben soll.

**Ein neuer Songtext**

> Schreib einen deutschen Indie-Pop-Song über meine erste Nacht in einer neuen Wohnung. Ich freue mich auf den Neuanfang, vermisse aber mein altes Leben. Der Refrain soll kurz sein. Bitte keine kitschigen Durchhalteparolen.

**Ein Refrain, der besser klingt**

> Überarbeite diesen Refrain. Die Zeile „Dein Schlüssel liegt noch neben mir“ soll bleiben. Der Rest darf schlichter und direkter werden. Ich möchte so klingen, als würde ich mit jemandem reden.

**Ein persönliches Lied**

> Ich möchte ein Geburtstagslied für meine Schwester schreiben. Sie wird 30, liebt Camping und kommt immer zu spät. Es soll liebevoll und lustig sein, mit einem Refrain, den alle mitsingen können.

**Ein Text für eine Melodie**

> Schreib vier Refrainzeilen mit jeweils acht gesungenen Silben. Das Betonungsmuster steht unten. Wenn eine Zeile nur mit falscher Wortbetonung passt, schlage eine andere Formulierung vor.

**Eine zweite Meinung**

> Lies meinen Songtext durch. Wo klingt das Deutsch unnatürlich? Wo wirkt ein Reim erzwungen? Zeig mir die Stellen und jeweils einen konkreten Vorschlag. Bitte schreib nicht gleich den ganzen Text um.

Ein [ausgearbeitetes Refrainbeispiel](beispiele/refrain.md) zeigt den Weg von der Idee zum Text, einschließlich Silbenzählung.

## Was du bekommst

Bei einem ganzen Lied erhältst du einen Titel und den Songtext mit klar gekennzeichneten Strophen und Refrains. Wenn du nur eine Zeile ändern möchtest, bleibt es bei dieser Stelle.

Für die weitere Musikproduktion kann der Skill Titel, Stilbeschreibung und Songtext getrennt ausgeben. Prüfanmerkungen und Erläuterungen stehen dabei außerhalb des Textes, der gesungen werden soll.

Liegt eine Melodie vor, werden ihre Vorgaben berücksichtigt. Ohne Melodie lässt sich prüfen, ob die Sprache flüssig ist und die Silbenzahl stimmt; wie die Wörter auf den Noten liegen, bleibt dann offen.

## Installation für Claude Code und OpenAI Codex

Der Skill besteht aus Markdown-Dateien und benötigt keine zusätzlichen Pakete oder API-Schlüssel. Kopiere den Ordner `deutsche-songtexte-skill` samt Unterordnern in das Skill-Verzeichnis deines KI-Assistenten.

Führe die folgenden Befehle aus dem übergeordneten Verzeichnis des Projektordners aus. Prüfe vorher, ob im Zielverzeichnis bereits eine eigene Fassung liegt.

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -R ./deutsche-songtexte-skill ~/.claude/skills/
```

Anschließend kannst du den Skill in Claude Code mit `/deutsche-songtexte-skill` aufrufen oder Claude direkt bitten, einen deutschen Songtext zu schreiben.

### OpenAI Codex

```bash
mkdir -p ~/.agents/skills
cp -R ./deutsche-songtexte-skill ~/.agents/skills/
```

In Codex kannst du den Skill ausdrücklich mit `$deutsche-songtexte-skill` ansprechen. Seine Beschreibung hilft dem Agenten außerdem, ihn bei passenden Aufgaben auszuwählen.

Die Installation richtet sich nach der offiziellen Dokumentation zu [Skills in Claude Code](https://code.claude.com/docs/en/skills) und [lokalen Skills in Codex](https://learn.chatgpt.com/docs/build-skills).

### Weitere KI-Assistenten

Bei anderen Assistenten, die das Format `SKILL.md` unterstützen, verwende das jeweilige Skill-Verzeichnis. Du kannst deinen Assistenten auch bitten, die [Anleitung in SKILL.md](SKILL.md) direkt zu lesen.

## Deinen Songtext vertonen

Der Text steht und du möchtest hören, wie ein Lied daraus klingt? Bei KlangKI kannst du mit deinem eigenen Text einen [KI-Song erstellen](https://kisongerstellen.com/):

1. Wähle auf der Website den Modus für eigene Songtexte.
2. Füge deinen Titel und den Text ein.
3. Beschreibe den gewünschten Klang, etwa „ruhiger Deutschpop mit Akustikgitarre und warmer Frauenstimme“.
4. Höre dir das Ergebnis an und verfeinere bei Bedarf den Text oder die Stilbeschreibung.

Du kannst auch mit einer Beschreibung beginnen oder reine Instrumentalmusik erstellen. Zum Schreiben mit diesem Skill brauchst du KlangKI nicht; du kannst die fertigen Texte ebenso in einem anderen Musikgenerator oder mit eigenen Musikern weiterbearbeiten.

## Inhalt

| Datei | Inhalt |
| --- | --- |
| [SKILL.md](SKILL.md) | Anleitung für den KI-Assistenten |
| [Sprache, Reime und Betonung](wissen/deutsche-songtexte.md) | Hinweise zum Schreiben deutscher Songtexte |
| [Refrainbeispiel](beispiele/refrain.md) | Ein kurzer Text mit nachvollziehbarer Silbenzählung |
| [LICENSE](LICENSE) | MIT-Lizenz |

## Lizenz

MIT, siehe [LICENSE](LICENSE).
