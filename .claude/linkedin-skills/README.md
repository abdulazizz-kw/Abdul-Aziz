# LinkedIn skills (vendored)

Source: https://github.com/sergebulaev/linkedin-skills (MIT, see `LICENSE`),
commit `261240ac5c4da8b4465cbd364d14ce52ffed12ce`.

Layout in this repo:

- `.claude/skills/linkedin-*` — the 12 skills Claude Code loads automatically
- `.claude/references/` — shared references the skills link to as `../../references/`
  (`voice-profile.md` and `story-bank.md` get filled with personal details; this repo
  is public, so keep filled copies out of git)
- `.claude/linkedin-skills/` — optional Python helpers (`lib/`, `scripts/`) for
  reading posts via Apify and publishing via Publora

Drafting works with no setup. For fetching/publishing, put `APIFY_TOKEN` and/or
`PUBLORA_API_KEY` in `.claude/linkedin-skills/.env` (git-ignored) and run
`pip install -r .claude/linkedin-skills/requirements.txt`, then
`python3 .claude/linkedin-skills/scripts/check_config.py` to verify.
