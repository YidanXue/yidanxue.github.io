# Yidan Xue's personal academic website

This repository is the static personal website at `yidanxue.github.io`. It is separate from the `ccimim.github.io` group website. Main files are `index.html`, `stylesheet.css`, `images/` and `data/CV_Yidan_Xue.pdf`.

## Required workflow for relevant tasks

Before reviewing or changing the website, read and follow [the update-yidan-website skill](.agents/skills/update-yidan-website/SKILL.md). It records the selective content, publication highlights, press links, CV synchronization and verification workflow. The user's current instructions take precedence.

For changes to CV source, read [the CV repository instructions](../CV_Yidan_Xue/AGENTS.md) and its linked skill first. The usual sibling path is `/Users/yidan/GitHub/CV_Yidan_Xue`; locate the real checkout if this repository is elsewhere. The downloadable website PDF is a copy, not the CV's editable source.

## Repository essentials

- Preserve the existing static HTML/CSS structure and inspect pending user changes before editing.
- Keep the stable CV download path `data/CV_Yidan_Xue.pdf` and verify copies against the intended source.
- Match requested scope; reviewing differences does not itself request implementation, and a private CV submission does not automatically request a public website entry.
- Verify branch and remote before synchronization or publication. `origin` is Yidan's repository; the historical `upstream` is an unrelated template source. Old chat approvals do not authorize new pushes or deployments; current-task authorization remains valid.

The skill lives in `.agents/skills/` for automatic Codex discovery. Agents without skill discovery should open the linked `SKILL.md` directly. Read the other skill only when the task calls for it.
