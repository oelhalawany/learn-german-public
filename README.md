# Meine Büro-Vokabeln

A small personal vocabulary page for practising spoken business German.

It is a single self-contained HTML file — no build step, no dependencies, no tracking, no external requests.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The vocabulary page — the actual site |
| `german-tutor-agent-instructions.md` | Reusable prompt defining how an AI agent should run German tutoring sessions |

### Using the tutor instructions

`german-tutor-agent-instructions.md` is a portable prompt. Paste it into any LLM or agent as a system
or custom instruction, and it will run tutoring sessions in the style described: casual spoken German
only, work-focused vocabulary, live inline corrections, and scenario-based exercises.

## Usage

Open `index.html` directly in your browser, or visit:

https://oelhalawany.github.io/learn-german-public/

## Adding words

Edit the `vocab` array inside the `<script>` block in `index.html`:

```js
{
  term: "der Aufwand",
  meaning: "the effort / work involved",
  sentences: [
    "Der Aufwand ist höher als gedacht.",
    "Wie viel Aufwand wär das ungefähr?"
  ],
  tag: "Meeting"
}
```

Each entry needs:

| Field | Description |
| --- | --- |
| `term` | The German word or phrase |
| `meaning` | Short English gloss |
| `sentences` | 2–3 example sentences in casual spoken German |
| `tag` | Category label shown on the card (e.g. `Meeting`, `Slack`) |

## Hosting

Published with GitHub Pages from the `main` branch, root folder.
