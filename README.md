# Small model, financial reports

A small open model (Gemma 3 4B) answers questions that need a figure worked out from a page of an annual report. 297 test questions from FinQA (Chen et al., 2021, MIT licence), restricted to banks, insurers and payment companies.

| Setup | Correct |
|---|---|
| Small model alone | 54% |
| + rules in code | no rule helped |
| + fine-tuning | 59% |

Fine-tuning helped one- and two-step questions and failed on questions needing three or more steps. The page (`index.html`) shows three example questions, the rules that were tried, the fine-tuning story, and every test question with its recorded answers, which the page replays on click. Nothing runs live.

Built from the recorded runs in the study repository by `site2/build.py`.
