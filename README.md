# RoboTeam media

Images, short clips, the film and the published results of
[RoboTeam](https://github.com/changxuanfan/RoboTeam), served from this repository's GitHub
Pages for the [project page](https://changxuanfan.github.io/RoboTeam/). Source code and
documentation live in the main repository.

The run videos themselves are in the Hugging Face dataset
[RoboTeam-Bench/RoboTeam-Videos](https://huggingface.co/datasets/RoboTeam-Bench/RoboTeam-Videos):
three camera views of every run, at ten times real time.

## What is here

| Path | Content |
| --- | --- |
| `posters/<set>/<task>-<view>.webp` | One poster per run for the front and the top view: the last frame of a completed run, otherwise a later frame of the run. `<set>` is a video set such as `gpt-6.1-sol` or `oracle`, `<task>` a task such as `transport-small-l1` |
| `clips/` | The short looping clips of the project page, with `spec.json` (what each clip is cut from) and `clips.json` (each clip's length and true playback speed) |
| `film/` | The RoboTeam film: a silent 30 s loop in two sizes with its poster, the long film, and `film.json`, which names the files |
| `findings.json`, `findings/` | The numbers behind the project page's charts, from the paper and its data tables, the per-step timelines of the gpt-6.1-sol and opus-5.5 runs, and one camera picture at full size and at 128 × 80 |
| `results.json` | The 14 conditions of the paper (tasks completed, tasks completed within 3, 6, 12 and 24 hours, median time and input tokens per task, median atomic failure rate) and, per video set, whether each of the 36 tasks was completed |

Posters and clips are made with `scripts/site/site_media.py` in the main repository, and the
formats of `results.json` and of the page's media index are described in its `site/DESIGN.md`.

Licensed under [CC BY 4.0](https://github.com/changxuanfan/RoboTeam/blob/main/LICENSE-DATA.md).
