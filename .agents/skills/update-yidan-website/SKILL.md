---
name: update-yidan-website
description: "Update or review Yidan Xue's personal academic website in yidanxue.github.io, including CV synchronization, publication rows, talks, roles, news links and local previews. Use for this personal GitHub Pages site, not the separate ccimim.github.io group website or a new Sites project."
---

# Update Yidan's personal academic website

Maintain the existing static portfolio and its selective academic presentation. These instructions distil the related chats through 28 October 2026 and the current repository conventions. Newer user instructions and verified current facts take precedence.

## Repository and scope

- The repository is `yidanxue.github.io`, normally `/Users/yidan/GitHub/yidanxue.github.io`. It is a compact static HTML/CSS website: `index.html`, `stylesheet.css`, publication thumbnails in `images/`, and the downloadable CV at `data/CV_Yidan_Xue.pdf`. Edit these sources directly; do not introduce a framework, migrate to Sites or revive the old al-folio template as part of a content update.
- The related CV source is the sibling `CV_Yidan_Xue` repository. Read its `AGENTS.md` and `update-yidan-cv` skill before changing CV source or bibliography. For a website-only comparison, read the CV as evidence, including relevant uncommitted updates.
- Distinguish requests to review/propose from requests to implement. Preserve explicit exclusions, including embargoed papers and narrow requests such as replacing only the downloadable PDF and updating talks.
- Inspect status/diffs in each repository being changed. Verify the actual branch and remote; historically the website uses `master`, while the CV uses `main`. The website's `upstream` remote points to a template, not Yidan's publishing destination. When a pull is requested, compare and fast-forward the appropriate `origin` branch, preserving pending work.

## Keep the website selective

- Preserve the existing layout, typography, profile image, section IDs, analytics, visitor map and footer attribution unless the task concerns them.
- Keep the profile concise and research-focused. Verify current appointments and affiliations rather than copying historical dates into new prose. Use British spelling except in official titles.
- Use `Talks` with `Speaking invitations` and `Contributed presentations`, usually newest first. Include meaningful event/series context and `online` where applicable. Do not reintroduce the removed five-minute internal lightning talk during a mechanical CV sync.
- Keep `Professional roles and memberships` selective. EMS topical-group and BSI Young Professionals memberships were deliberately omitted from the website; do not add them automatically just because they are in the CV. Committee subgroups can be unbulleted `<br>` continuations inside the parent `<li>`.
- Put selected organising/presenting activities and webinar recordings under `Miscellanea`. Do not automatically create a separate scientific-leadership section or copy the full CV service/mentoring history. A completed event should not retain an `incoming` label; decide whether to retain a completed highlight or remove a transient announcement in the scope of the requested update.
- Use informative, concise link labels such as `recording`, `registration`, `code` and `web app`, linking to official sources where available. Avoid duplicating the same activity as both an invited talk and an organising duty without evidence of distinct roles.

## Publication rows and press links

- Follow neighbouring `tr.paper` rows: thumbnail, linked title, full author list in paper order with `<strong>Yidan Xue</strong>`, italic venue and year, useful resource links, then a concise evidence-based description. Do not invent findings or numerical claims from the title alone.
- The current selection convention highlights all first- and co-first-authored papers using `class="paper highlighted"`; other rows use `class="paper"`. Respect an explicit selection override. Do not invent a `selected` field in this static HTML site.
- Use verified titles, authors, dates and final DOI links. Preserve official title typography (for example `<em>in silico</em>` in the Device title). Clearly distinguish published, accepted and public-preprint status. Reconcile an existing row when a preprint is published rather than adding a duplicate.
- Apply the CV skill's authorship-symbol rule if symbols are needed: show Yidan's relevant credit, not unrelated corresponding-author metadata. Keep full given names on the website instead of converting the author list to CV initials.
- A private submission listed in the CV does not automatically become a public website entry. Check the requested scope and any publication/embargo restriction. Do not copy accepted manuscripts, supplementary information or submission packages onto the website merely because they were supplied for reference; the user has specifically preferred publisher links over these uploads.
- Prefer a supplied or published figure that remains legible at the existing thumbnail width (about 160 px). Preserve aspect ratio, use descriptive alt text, and check cropping at actual display size. Do not fabricate a scientific result as a decorative thumbnail.
- Keep selected press links under their relevant publication, as the repository now does for Device and VIRIS. Do not recreate a separate media/Selected Press section or import every CV news item by default. Verify that each linked article actually covers the associated work.

## Synchronize the downloadable CV

1. Identify the intended source: use an explicitly supplied final PDF when requested; otherwise use the current verified `CV_Yidan_Xue/main.pdf`. If rebuilding the CV is part of the task, follow its skill first.
2. Copy it to `data/CV_Yidan_Xue.pdf`, preserving that filename and the existing public link. Do not reflow, compress or repaginate a supplied PDF unless asked.
3. Verify byte equality with the intended source (`cmp` or a cryptographic hash), and check that the site link resolves to the copied file. File timestamps alone are insufficient.

## Verify and publish within the requested scope

- Check the HTML structure, local links/images, special characters, title/author accuracy and highlight classes. Preview affected sections at desktop and narrow/mobile widths when layout or content wrapping changes. A successful file edit or HTML parse alone is not visual verification; report if a browser preview is unavailable.
- For a PDF-only copy, verify file identity and the download link; a full website build is unnecessary. This static site has no required npm build.
- Update `Last updated: Month YYYY` when public content is changed, using the user's current date/time zone. Do not update it for instruction-only edits.
- Run `git diff --check`, review the final scope, and report local/committed/pushed status. Keep `.DS_Store` and preview artifacts out of commits.
- Commit/push/deploy when authorized for the current task; do not treat an earlier chat's approval or one-off release schedule as permanent permission. When publishing is requested, verify the correct GitHub destination and the deployment/live content before claiming the website is live. Scheduled pushes use the user's specified Europe/London time and require an actual supported scheduling mechanism; do not silently substitute an immediate push.
