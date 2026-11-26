# selfplay-next

A policy trained with PPO and self-play (python/train/ppo.py in the game's repository), exported with python/train/export.py.
Each row is a version: it was entered only when it beat the one before with 95% confidence, over games played
under league conditions (sampled actions, every seed from both sides).

| Date | Update | Env steps | Checkpoint | Against the version before |
| --- | --- | --- | --- | --- |
| 2026-11-25 | 18740 | 835 M | `runs/rules4-c/latest.pt` | first version: no comparison |
| 2026-11-25 | 19510 | 870 M | `runs/entry-a/latest.pt` | 228-1-123 against update 18740 (64.9%, 95% interval 59.8%-69.7%); entered before this comparison finished, to make the 2026-11-26 tournament |
| 2026-11-25 | 19510 | 870 M | `runs/entry-a/latest.pt` | 171-1-92 against update 18740 (65.0%, 95% interval 59.0%-70.5%) |
