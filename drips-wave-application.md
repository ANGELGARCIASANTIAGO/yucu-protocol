# Drips Wave application: class diagram of the payout port (Yucu)

Guide and draft application for the issue "Draw a class diagram of the payout port and its data" in the Open-Hub-Tec/yucu-protocol repository (Good first issue · design · no coding required · Trivial · 100 pts).

## 1. How to apply

According to the repository's `CONTRIBUTING.md`:

1. Sign in at drips.network/wave with your GitHub account.
2. When a Wave is active, find the Yucu issue in the Drips app and **apply there**. A comment on GitHub alone is not an application.
3. Wait for the maintainer to assign you the issue. **Do not start before that.**
4. Open your PR with `Resolves #<issue number>`. Each Wave lasts one week.

## 2. Requirements to receive the reward

- Be 18 or older.
- Pass Drips' identity check (KYC).
- For teams, one person applies and Drips pays that person; how the team shares the reward is the team's own decision.
- There is no guaranteed reward, amount or date.
- For TecNM Campus Tlaxiaco students, taking part is voluntary and your course grade does not depend on applying, passing the identity check or receiving a reward.
- Drips does not accept low-quality, untested or AI-generated work that you do not understand: in the review you will have to explain every part of the diagram.

## 3. Application message (paste into Drips)

Replace the text in brackets with real information and do not claim anything that is not true.

> Hi! I'd like to take this issue: "Draw a class diagram of the payout port and its data".
>
> I have read AGENTS.md, CONTRIBUTING.md and src/core/chain/ports.ts. My plan:
> 1. Draw only what ports.ts defines (PayoutPort, PayoutQuote, CashoutRequest, CashoutReceipt, PayoutState, PayoutStatus), plus the supporting types they reference, and write anything undefined as a note instead of inventing it.
> 2. Build the diagram in [Modelio / Enterprise Architect] and export it as a PNG at least 800 px wide.
> 3. Add docs/uml/clases-cobros.md (title, short explanation, image, Elements table, sources) and docs/uml/img/clases-cobros.png, following docs/uml/README.md.
> 4. Open the PR with "Resolves #<issue number>" and make sure the "Validar diagramas UML" check is green.
>
> I can finish within the Wave week. I will only start after I am assigned, and I can explain every part of the diagram in the review.
>
> [Optional: one line about you, e.g. "I'm a student at TecNM Campus Tlaxiaco, Fundamentos de Ingeniería de Software."]

## 4. Checklist before sending

- [ ] I read `AGENTS.md`, `CONTRIBUTING.md` and `src/core/chain/ports.ts`.
- [ ] I have Modelio (free) installed, or a licensed copy of Enterprise Architect.
- [ ] Nobody else is assigned to the issue (one person per issue).
- [ ] I am 18 or older and willing to pass the identity check if I want to receive the reward.
- [ ] My message only says things that are true.

## 5. After you are assigned

Files to add (and nothing else):

- `docs/uml/clases-cobros.md`
- `docs/uml/img/clases-cobros.png` (at least 800 px wide, exported from Modelio with "Save diagram in a file")
- Optional: `docs/uml/modelos/clases-cobros.xmi`

Do not upload Modelio or Enterprise Architect project files.

Commands:

```bash
git checkout -b docs/uml-clases-cobros
mkdir -p docs/uml/img
git add docs/uml/clases-cobros.md docs/uml/img/clases-cobros.png
git commit -m "docs(uml): add class diagram of the payout port"
git push origin docs/uml-clases-cobros
```

PR body (the first line is required):

```
Resolves #<issue number>

Adds a class diagram of PayoutPort and its data, drawn only from
src/core/chain/ports.ts. Includes PayoutPort, PayoutQuote, CashoutRequest,
CashoutReceipt, PayoutState and PayoutStatus with their real fields and methods.
No drawing-tool project files are included.
```

## 6. Sources

- `CONTRIBUTING.md`, section "Applying through Drips Wave", in the Open-Hub-Tec/yucu-protocol repository.
- The issue text.
