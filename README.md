# RoboTeam media

Videos and published results of [RoboTeam](https://github.com/changxuanfan/RoboTeam), served
from this repository's GitHub Pages for the
[project page](https://changxuanfan.github.io/RoboTeam/). Source code and documentation live in
the main repository.

## Video sets

Each video set is one folder. A set holds one run of each of the 36 released tasks, and every
set uses the same file names.

| Folder | Runs | State |
| --- | --- | --- |
| `oracle/` | The Oracle: gpt-6.1-sol in Codex as a single agent, given the ground-truth position of every object instead of camera images. Some recordings were operator-assisted | Published |
| `gpt-6.1-sol/` | gpt-6.1-sol in Codex with the adaptive system | Not yet published |
| `opus-5.5/` | opus-5.5 in Claude Code with the adaptive system | Not yet published |
| `kimi-k3.1-pro/` | kimi-k3.1-pro in Codex with the adaptive system | Not yet published |
| `qwen3.8-flash/` | qwen3.8-flash in Codex with the adaptive system | Not yet published |
| `deepseek-v4.1-flash/` | deepseek-v4.1-flash in Codex with the adaptive system | Not yet published |
| `glm-5.3-flash/` | glm-5.3-flash in Codex with the adaptive system | Not yet published |

Files in a set:

| Path | Content |
| --- | --- |
| `<task>-front.mp4`, `<task>-side.mp4` | The run from the front and from the side, rendered in the factory hall, 720p H.264. `<task>` is the released task id, for example `transport-small-l1` |
| `<task>-<view>.jpg` | Poster frame of each video |
| `manifest.json` | Size, duration and SHA-256 of every file, and the SHA-256 of its 1080p source render |

The Oracle recordings were rendered before the tasks got their released ids, so the signs on
the floor show the earlier names (for example `TRANSPORT-A08-D1` for `transport-medium-l1`).

Videos were encoded with `scripts/site/site_media.py` in the main repository (libx264, CRF 28,
preset slow, faststart).

## Results

| Path | Content |
| --- | --- |
| `results.json` | The 14 conditions of the paper (tasks completed, tasks completed within 3, 6, 12 and 24 hours, median time and input tokens per task, median atomic failure rate) and, per video set, whether each of the 36 tasks was completed and how long the run took |

The file's format is described in the main repository's `site/DESIGN.md`.

## Film

A tour of the factory hall, cut from Oracle reference runs. It does not show model results.

| Path | Content |
| --- | --- |
| `film/roboteam-film-1080p.mp4` | The film, 3 min 41 s, 1080p: one moment from each zone, then every task type and team size |
| `film/roboteam-short-1080p.mp4` | The short cut, 25 s, 1080p: the title card, one moment from each zone and the hall |
| `film/film.jpg` | Poster frame of the film |

Licensed under [CC BY 4.0](https://github.com/changxuanfan/RoboTeam/blob/main/LICENSE-DATA.md).
