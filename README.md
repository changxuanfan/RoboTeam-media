# RoboTeam media: Oracle reference videos

Video files for the [RoboTeam project page](https://changxuanfan.github.io/RoboTeam/),
served from this repository's GitHub Pages. Source code and documentation live in
[changxuanfan/RoboTeam](https://github.com/changxuanfan/RoboTeam).

| Path | Content |
| --- | --- |
| `oracle/<task>-front.mp4`, `oracle/<task>-side.mp4` | Oracle reference run of each of the 36 released tasks, rendered in Robo World, 720p H.264. The Oracle is gpt-6.1-sol in Codex as a single agent with ground-truth object positions; some recordings were operator-assisted |
| `oracle/<task>-<view>.jpg` | Poster frame of each video |
| `oracle/manifest.json` | Size, duration and SHA-256 of every file, and the SHA-256 of its 1080p source render |
| `film/robofrontier-film-1080p.mp4` | The earlier 3 min 41 s tour of Robo World, 1080p: one moment from each zone, then every family and scale |

Videos were encoded with
`scripts/site_media.py` in the main repository (libx264, CRF 28, preset slow, faststart).

Licensed under [CC BY 4.0](https://github.com/changxuanfan/RoboTeam/blob/main/LICENSE-DATA.md).
