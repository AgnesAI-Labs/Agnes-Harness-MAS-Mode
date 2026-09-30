# Agnes Harness MAS Mode

## Recursive Self-Improvement for Multi-Agent Systems

Agnes Harness MAS Mode uses a GLM 5.3 Flash planner and an Agnes 2.5 Flash helper. It learns from task traces in two ways: a helper profile informs future delegation, and harness rules enforce behaviors that prompt instructions alone did not reliably produce.

This repository publishes the article by @Aiden, dated September 29, 2026. The results are from internal testing on terminal tasks and a small SWE-bench Verified sample. They should be read with those evaluation limits in mind.

## Read the article

- [Full article with figures and tables](REPORT.md)
- [PDF edition](PAPER.pdf)

## Reported findings

- On the internal Terminal-Bench 4.0 tasks, MAS Mode matched GLM 5.3 Flash working alone on average task score at **48% lower cost** across completed attempts.
- On the first attempt at each task, its cost was **51% lower**, and the planner used **68% fewer tokens** than GLM 5.3 Flash working alone.
- Agnes 2.5 Flash fully solved none of the tested terminal tasks alone and seven when paired with the planner. On a small SWE-bench Verified sample, the pair resolved 13 of 15 issues versus 9 of 15 for the helper alone.
- Across measured RSI rounds 0–3, the helper's token share rose from about one third to 60%. Rounds 4 and 5 shown in the article are targets, not measured results.

The article explains the evaluation definitions, pricing assumptions, delegation rules, failure cases, and the boundary between measured rounds and future targets.

## Publication note

The PDF was rendered from the supplied Word article with slightly adjusted page margins so the final paragraph stays with the rest of the article. The text, figures, tables, and reported findings were preserved. The Markdown edition transcribes the supplied article and includes its five original figures.
