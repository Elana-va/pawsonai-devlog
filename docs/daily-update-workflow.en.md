# PAWSON AI Public Development Log · Daily Workflow

[简体中文](daily-update-workflow.md) · **English**

This workflow defines how PAWSON AI turns daily activity in the private source project into a safe public development journal. It explains why the product changed, what was actually completed, how it was verified, and what remains limited while protecting source code, credentials, customers, and internal systems.

## Publishing cadence

- Run one public review and update for every Asia/Shanghai calendar day.
- Combine multiple development events into one entry organized around a clear theme.
- When no public, verified milestone exists, publish a short status entry marked “in progress,” “internal-only work,” or “no new verified result.” Never invent progress.
- When a major release, roadmap change, or important verification result appears, update the homepage, development story, roadmap, or release notes as well.
- Publish the Chinese and English editions together.

## Daily inputs

The journal starts from evidence rather than reconstructing results from plans or memory. Valid inputs include:

1. The private repository's commits, current branch, and worktree status for the day.
2. Acceptance notes, tests, builds, smoke checks, and manual verification from completed tasks.
3. Product interfaces, real output files, and approved milestone screenshots.
4. Recorded technical decisions, known limits, and next steps.
5. The previous public entry, to avoid repeating old work as today's progress.

Uncommitted changes may support an “in progress” statement, but they are not delivered results. UI messages, placeholders, local caches, and plans cannot prove success by themselves.

## Step 1: Build the day's fact list

Classify the material into four groups:

| Category | What it may contain | Writing rule |
| --- | --- | --- |
| Completed | Product changes with supporting evidence | Use past tense and explain user value |
| Verified | Tests, builds, real files, or manual acceptance | State public counts, scope, and limits |
| In progress | Work that started but is unfinished | Label it clearly; do not present it as a result |
| Known limits | Failures, external dependencies, and unresolved issues | Explain the impact; do not hide failures |

When evidence conflicts, prefer reviewable code, files, test output, and remote state. Put uncertain claims under “to verify” or leave them out.

## Step 2: Extract the public story

Choose one theme that an outside reader can understand instead of listing internal filenames. A useful entry answers six questions:

1. Why did we work on this today?
2. What problem existed before?
3. What was actually completed or confirmed?
4. Which product or engineering decisions were made?
5. What evidence and real limits exist?
6. What will be verified next?

Entries may discuss product capabilities, user experience, milestone screenshots, public test counts, and non-reproducible design reasoning. Avoid copying Git commits line by line; commit messages often expose internal module names and rarely explain user value.

## Step 3: Run the redaction check

The public repository must not contain:

- Source code, complete diffs, full system architecture, or reproducible core algorithms.
- API keys, tokens, cookies, passwords, key files, or real test credentials.
- Provider addresses, internal APIs, server IPs, admin URLs, ports, or deployment configuration.
- Database schemas, migration details, real business data, or internal billing rules.
- Customer names, user accounts, conversations, orders, contact details, or personal information.
- Browser profiles, absolute local paths, private repository addresses, or undisclosed partners.
- Full system prompts, security bypass instructions, or internal risk-control details.

If a detail's sensitivity is unclear, do not publish it. Replace it with the product impact, verification conclusion, or an abstract implementation direction.

## Step 4: Prepare project images

Use images only when they explain a real product change:

1. Select an interface, output, or comparison directly related to the day's theme.
2. Inspect window titles, browser tabs, avatars, notifications, paths, filenames, and admin addresses.
3. Crop unrelated desktop areas and mask anything that cannot be public.
4. Remove EXIF, XMP, IPTC, GPS, software paths, and other metadata.
5. Use a generic filename such as `2026-09-agent-workspace.png`.
6. Add accurate alt text and a short caption in both language editions.

An image cannot be the only proof of completion. External-service claims also require reviewable runtime state, output files, or logs.

## Step 5: Write both language editions

Create a pair of files for each date:

```text
updates/YYYY-MM-DD.md
updates/YYYY-MM-DD.en.md
```

Link the pages to each other at the top. Both editions must preserve the same facts, numbers, limits, and next steps. Adapt the English version for natural English reading instead of translating mechanically line by line.

Use the [Chinese template](../updates/TEMPLATE.md) and [English template](../updates/TEMPLATE_EN.md):

- Why
- What was completed
- Key decisions
- Verification evidence
- Known limits or items still to verify
- Next

Use a title that describes the change, such as “The Agent began handling files and long-running work.” Avoid empty titles such as “Today's update” or “Continued optimization.”

## Step 6: Update navigation and long-lived documents

Every entry updates at least:

- `updates/README.md`: Chinese date index.
- `updates/README_EN.md`: English date index.
- `README.md` and `README_EN.md`: homepage latest-update links and current status.

Update longer-lived documents when their trigger occurs:

| Trigger | Update |
| --- | --- |
| The product direction, key decision, or stage narrative changes | Both development-story editions in `docs/` |
| Priorities or public plans change | `ROADMAP.md` and `ROADMAP_EN.md` |
| A user-visible change deserves quick reference | Both changelog editions |
| A defined delivery version is formed | Both release pages under `releases/` |
| A safe public interface visual is added | The gallery indexes under `screenshots/` |

## Step 7: Validate before publishing

Complete these checks before publication:

- Dates, numbers, versions, and completion states match their evidence.
- Chinese and English facts match, and pages link to each other.
- Relative links, image paths, and indexes resolve.
- Markdown formatting has no broken tables or empty links.
- Text contains no credential patterns, internal addresses, customer data, or absolute paths.
- Images pass visual review and metadata inspection.
- The Git diff contains only files required for this public entry.

If any check fails, keep a local draft and do not push a partial entry.

## Step 8: Commit, publish, and verify remotely

Recommended commit message:

```text
docs: publish YYYY-MM-DD development journal
```

After pushing the public repository, verify that:

1. GitHub `main` points to the new commit.
2. Both language editions are reachable from their indexes.
3. The homepage latest-update links point to today's pages.
4. Images render and language switching returns the matching page.
5. The local branch matches the remote and contains no temporary publishing files.

The daily entry is published only after remote verification succeeds. If the network or push fails, preserve the local commit and retry; never describe a local-only commit as publicly available.

## Daily definition of done

A daily update is complete only when it is:

- Truthful: completed claims have evidence, and ongoing or failed work is not disguised as success.
- Safe: text, links, and images pass redaction checks.
- Bilingual: both editions and navigation are synchronized.
- Readable: an outside reader can understand the problem, change, impact, and next step.
- Reachable: remote pages, images, and language switching have been verified.

The workflow may evolve with the project, but four principles remain fixed: evidence first, no sensitive information in public assets, bilingual synchronization, and remote confirmation before declaring publication.
