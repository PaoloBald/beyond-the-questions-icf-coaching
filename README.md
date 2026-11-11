# Beyond the Questions
### An Ontological Reflection Skill for Coaches

> **Not to tell coaches how well they performed, but to help them discover what they were unable to see.**

*Beyond the Questions* is an open set of instructions that turns a general AI assistant (Claude, ChatGPT, Gemini, Copilot and others) into a **reflective practice partner** for professional coaches.

You bring an anonymized session excerpt or a remembered moment. The assistant does not grade you. It picks out the moments worth looking at and asks you questions, one at a time, about what you noticed, assumed, felt and wanted, using the **ICF Core Competencies** as a lens and **ontological coaching** distinctions as tools.

---

## Why another AI tool for coaches?

Several tools already analyze coaching sessions against the ICF competencies and PCC markers. They answer one question: *did the coach apply the competencies?*

This project asks another: **from which observer did the coach act?**

| AI Evaluator | AI Reflective Partner (this project) |
|---|---|
| "You demonstrated Competency 7 in 70% of opportunities." | "What did you notice in the client when you chose not to explore that answer?" |
| Works on behaviour | Works on the observer behind the behaviour |
| The coach tries to improve a score | The coach discovers a new distinction |
| Single-loop learning | Double-loop learning |

Ontological coaching holds that sustainable change in results comes from a change in the *observer*. This project applies that principle to the coach's own professional development.

## A 30-second example

> **Client:** "I can't delegate because nobody is competent enough."
> **Coach:** "What could you do to improve your team's skills?"

An evaluator might tag the question under *Evokes Awareness*. *Beyond the Questions* asks the coach instead:
- "What interpretation of the situation did your question quietly accept?"
- "Did you hear 'nobody is competent enough' as a fact or as a judgment?"
- "What might have become possible if you'd explored the client's relationship with control?"

See `examples/` for full worked cases.

---

## How to use it

### Claude (claude.ai, Claude Desktop, Claude Code)
1. Download this repository as a ZIP (or zip the folder yourself).
2. In Claude: **Settings → Capabilities → Skills → Upload skill** and upload the ZIP. (The menu location may change. See Anthropic's Help Center on Skills.)
3. Start a chat: *"I'd like to reflect on a coaching session"* and paste your anonymized excerpt.

### ChatGPT
- **Custom GPT:** paste `prompt/chatgpt-gpt-instructions.md` into *Instructions*, and upload `prompt/universal-system-prompt.md` as a knowledge file.
- **Project:** put `prompt/universal-system-prompt.md` in the project instructions, or upload it as a file.

### Gemini, Copilot, Mistral, local models
Paste `prompt/universal-system-prompt.md` as the system prompt or custom instructions (for example a Gemini *Gem*).

### Before your first session
Read [`ETHICS_AND_BOUNDARIES.md`](ETHICS_AND_BOUNDARIES.md), especially the section on anonymization and the data settings of your AI provider.

---

## The method in one page

| Phase | What happens |
|---|---|
| **0. Contract** | What do you want to look at? What would make this useful? Confidentiality check. |
| **1. Locate moments** | The assistant picks 2 to 4 significant moments (agreements, listening, questions, silence, emotions, judgments, action), each linked to an ICF competency, **without evaluation**. You choose where to start. |
| **2. Reflective dialogue** | One question at a time through seven layers: fact → observation → interpretation → emotion and body → agenda → action space → way of being. At most one distinction is offered, as a hypothesis. |
| **3. Integration** | What do you see now? What distinction do you keep? What will you try next time? What goes to supervision? |
| **4. Log** | Optional reflection log in your own words (`templates/reflection-log.md`). |

Three levels of learning: **doing** (a new intervention), **observer** (a new distinction), **being** (a revised belief about coaching, clients or self).

---

## Repository structure

```
beyond-the-questions/
├── README.md                        ← you are here
├── SKILL.md                         ← the skill (Claude format; readable by any LLM)
├── ETHICS_AND_BOUNDARIES.md         ← confidentiality, consent, limits
├── LICENSE.md                       ← CC BY 4.0
├── references/
│   ├── icf-competency-lens.md       ← the 8 ICF Core Competencies as a lens for noticing
│   └── ontological-distinctions.md  ← OAR, BEL, speech acts, facts vs judgments, moods…
├── templates/
│   └── reflection-log.md            ← personal log for each reflection
├── prompt/
│   ├── universal-system-prompt.md   ← everything in one file, for any assistant
│   └── chatgpt-gpt-instructions.md  ← short loader for a ChatGPT Custom GPT
└── examples/
    ├── case-01-delegation.md
    ├── case-02-goal-drift.md
    └── case-03-silence-and-rescue.md
```

## What this is not
- **Not an assessment.** It never scores sessions or says whether a PCC marker was met.
- **Not supervision or mentor coaching.** It complements them.
- **Not affiliated with or endorsed by ICF.** Competency descriptions are paraphrases. Refer to ICF for official texts.

## Theoretical background
Ontological coaching (Echeverría, *Ontología del lenguaje*, 1994), Maturana & Varela's biology of cognition (*The Tree of Knowledge*), reflective practice (Schön, *The Reflective Practitioner*, 1983), double-loop learning (Argyris & Schön, 1974), and the supervision literature (Hawkins & Shohet). See `references/ontological-distinctions.md` for the full list.

## Author
**Paolo Baldriga**, ICF PCC, co-author (with Raquel Guarnieri) of *Coaching and Neuroscience*.

## Contributing
Issues and pull requests are welcome, especially new anonymized/fictional examples, translations and field reports from coaches and supervisors. Please never submit real client material.

## License
CC BY 4.0. See [`LICENSE.md`](LICENSE.md).
