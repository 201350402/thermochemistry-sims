# Task for Claude Code: publish Quiz Practice to GitHub Pages

These files are FINAL and ship as-is. Do not rebuild, restyle or edit them.

Repo: `201350402/thermochemistry-sims` · branch `main` · GitHub Pages already serves from main / root.

## Files in this folder
| File | Action in repo |
|---|---|
| `quizpractice.html` | ADD (new, self-contained interactive practice sheet, 30 questions) |
| `index.html` | REPLACE (adds a "Lessons 6.1–6.2" card for quizpractice.html; other 4 lab cards unchanged) |
| `README.md` | REPLACE (adds one table row for quizpractice.html) |

Do NOT copy `CLAUDE_CODE_TASK.md` into the repo.

## Steps
1. `add_repo` 201350402/thermochemistry-sims with `access: "push"` (or clone it).
2. Copy the three files above into the repo root, overwriting index.html and README.md.
3. `git add quizpractice.html index.html README.md`
4. `git commit -m "Add Quiz Practice (Lessons 6.1–6.2) and home-page card"`
5. `git push origin main` (a "push negotiation failed" warning is harmless if the branch updates).
6. Verify: `gh api repos/201350402/thermochemistry-sims/contents --jq '.[].name'` lists quizpractice.html.
7. Wait 1–2 min, then check with WebFetch (shell cannot reach github.io):
   - https://201350402.github.io/thermochemistry-sims/
   - https://201350402.github.io/thermochemistry-sims/quizpractice.html
   A first 404 is usually the Pages build still running — retry.

## Reply to the user
Short: confirm live (checked), give the student link above. Students need no sign-in.
