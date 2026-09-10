# PAWSON AI Daily Development History

[简体中文](daily-development-history.md) · **English**

> Organized by Asia/Shanghai calendar date. Last updated: September 10, 2026.

**Quick jump:** [Latest committed development day](#latest) · [September 9](#day-2026-09-09) · [September 8](#day-2026-09-08) · [September 7](#day-2026-09-07) · [Home](../README_EN.md)

This timeline follows PAWSON AI on the private source repository's actual commit dates. Ordinary development days receive a concise note, while major feature, architecture, and release days expand to about seven or eight points. Dates without commits are omitted.

## July 2026

### July 27 | From local tools to a commercial-client foundation

- Created the first formal commits in the private source repository.
- Established payment configuration, administration APIs, and console foundations.
- Added signing, notification, and result verification for WeChat Native payments.
- Removed manual payment routes that could not provide authoritative settlement evidence.
- Connected the packaged client to the cloud control center.
- Added device, plan, and backend-service configuration boundaries.
- Released the 1.0.5 local acceptance build while documenting remaining launch gaps.

### July 28 | Accounts, releases, and production reliability

- Added provider model discovery to reduce fixed model configuration.
- Added desktop release publishing, upload progress, and self-service administrator management.
- Added password changes and automatic refresh for expired administrator sessions.
- Unified tool-page containment and result previews.
- Adjusted image-task timeouts and packaged-client connectivity.
- Prevented duplicate paid submissions and warmed the local background-removal runtime.
- Prepared copyright and payment handoff materials without treating documents as business acceptance.

### July 30 | Unified product-image production workspace

- Brought generation, task selection, and result presentation into one production workspace.
- Added continuation from single results and galleries into downstream image tools.
- Added idempotent result handoff to prevent duplicate operations.
- Restored task parameters without charging again and stopped retries for explicitly rejected requests.
- Reconciled task state after connection recovery and made failures actionable.
- Validated exports and production error classes while preserving valid results.
- Prepared version 1.1.0 and moved from isolated tools toward a continuous production flow.

### July 31 | The golden production path

- Defined one repeatable core image-production acceptance path.
- Added a production journey bar and journey state model.
- Began carrying explicit context across pages while guarding unsafe cross-step actions.

## August 2026

### August 1 | Local print extraction entered internal testing

- Prepared the 1.1.1 internal test build.
- Designed local garment-print extraction.
- Corrected extraction to use only the user-selected print region.
- Prepared the 1.1.2 print-extraction test build.

### August 2 | Production became project-centered

- Organized assets, parameters, tasks, and results around recoverable projects.
- Defined model-routing ownership so individual pages did not choose providers independently.
- Stopped retrying requests explicitly rejected by providers.
- Added an alignment implementation plan and release handoff.
- Prepared version 1.1.3.
- Project-centered work became the base for product details, data assets, and long-running tasks.

### August 6 | Development model routing changed

- Updated the Codex model routing used for development tasks.
- This changed development tooling, not the product's public capability.

### August 9 | Stable business-loop baseline

- Saved a recoverable checkpoint before parallel development.
- The checkpoint protected the working business loop but did not itself represent a feature release.

### August 10 | Stable report-delivery baseline

- Saved the enterprise-collaboration report checkpoint before further UI work.
- Established a clear rollback point for report reading and delivery changes.

### August 12 | Reports became real deliverables

- Improved the report center's reading, organization, and delivery experience.
- Connected report output to enterprise collaboration tools.
- Governed cross-border worker artifacts so temporary results did not become formal assets.
- Added platform and cross-border handoff records.
- Details: [Reports became real deliverables](../updates/2026-08-12.en.md).

### August 13 | Stable RC feature checkpoint

- Saved the verified feature baseline before overnight interface changes.
- The checkpoint supported recovery and comparison without expanding public capability claims.

### August 16 | Baseline before product-detail planning

- Saved a stable PAWSON RC checkpoint before the product-detail planner.
- Existing reports, tasks, and production capabilities gained a clear rollback point.

### August 18 | PAWSON Agent v0.5 checkpoint

- Saved the Agent v0.5 stage build.
- Began bringing image production and business capabilities into a unified conversation entry point.
- Runtime recovery and real task completion still required further work.

### August 20 | Visual answers and transport recovery

- Made visual answers lead with user-visible evidence.
- Defined transport observability and recovery.
- Saved the vision-run and transport-recovery checkpoint.
- Created failure evidence for the following Agent MVP stabilization.

### August 21 | The Agent MVP became the main product line

- Established persistent conversation and task-state foundations.
- Combined specialist capabilities with conversation context.
- Stabilized failure recovery and input preservation.
- Saved the PAWSON Agent MVP v0.5 baseline.
- Details: [The Agent MVP became the primary product line](../updates/2026-08-21.en.md).

### August 22 | Multi-task and context foundations

- Established independent state for multiple PAWSON tasks.
- Improved conversation history and Agent interaction.
- Stabilized concurrent tasks and expert conversations.
- Hardened Skill, expert, and session boundaries.
- Saved local acceptance and context checkpoints.
- Prepared data, knowledge, and collection as trusted Agent context.

### August 23 | Data, knowledge, and web collection foundations

- Established the core data foundation.
- Established the knowledge foundation.
- Integrated the core web-collection schema with provenance.
- Refined the expert-center experience.
- Simplified the Agent constitution to reduce ambiguity across tasks.

### August 24 | Data assets became a product capability

- Established the PAWSON 2.0 product-surface foundation.
- Connected data assets to real core data rather than placeholders.
- Connected knowledge to the same core data.
- Allowed operations work to register data assets explicitly.
- Added data-asset and knowledge read models.
- Preserved page state across navigation and application restarts.
- Refined the data overview while keeping provenance and access boundaries.

### August 25 | Knowledge management and unified controls

- Added real knowledge-base creation and lifecycle management.
- Allowed data assets to enter and leave knowledge bases safely.
- Added stable display identity for knowledge items.
- Managed expert access to knowledge bases.
- Reshaped the expert center and knowledge-management surface.
- Unified dropdowns across production, imports, tasks, operations, and listings.
- Aligned data and production workspace styling and improved global insights readability.
- Hardened management access so UI state could not expand permissions.

### August 26 | Collection, data, and product projects connected

- Brought the data collection center into the product interface.
- Added a persistent browser collection runtime and safe product-data service.
- Turned product trends, channels, and traffic into readable product capabilities.
- Registered collected results as data assets with provenance.
- Created an isolated, editable product-detail project prototype.
- Used text and image generation for product-detail drafts.
- Refined expert identity and the conversation rail.
- Details: [Collection, data, and product projects became connected](../updates/2026-08-26.en.md).

### August 27 | Unified workspace and expert creation

- Consolidated the PAWSON workspace shell.
- Built the expert-creation data model and complete wizard.
- Made product-detail posters independently editable.
- Refined operations signals and navigation.
- Aligned collection, search, and data visual hierarchy.
- Updated state and task handoff records.
- Removed contracts for product-detail paths that had left the main line.

### August 28 | A general, file-aware Agent

- Upgraded the Agent from fixed Q&A to a tool-driven general core.
- Added bounded file input with type, size, and workspace limits.
- Added explicit recovery for transport failures.
- Resumed sensitive tools only after user approval.
- Moved selected external-tool ownership into the Agent SDK boundary.
- Completed integration verification and recovery fixes.
- Established the base for commands, long-running work, and file delivery.

### August 29 | Global assistant and recoverable product-detail projects

- Defined product-detail project format and autosaved history.
- Added project import, export, copy, recovery, and continued editing.
- Added the project-library API and visual project list.
- Ran the global assistant in an isolated session with current-page context.
- Kept the page assistant separate from formal main-task history.
- Hardened provider recovery, global analysis, and draft quarantine.
- Reduced idle work and redundant commercial task polling.
- Merged parallel product-detail and guide work and satisfied build contracts.

### August 30 | Demo and recovery cleanup

- Added the product demo guide.
- Condensed conversation bootstrap state.
- Continued hardening provider retry and recovery boundaries.

## September 2026

### September 1 | The Agent began handling files and long-running work

- Defined controlled local command contracts and command-line-first execution.
- Executed bounded commands and verified real produced files.
- Preserved state, stopping, recovery, and valid artifacts across long runs.
- Made file cards openable and durable across application restarts.
- Loaded document and spreadsheet Skills with visible loading state.
- Added external Skill registration, discovery, inspection, and mounting.
- Bounded GitHub Skill inspection and reduced unnecessary model turns.
- Details: [The Agent began handling files and long-running work](../updates/2026-09-01.en.md).

### September 2 | Official NEW PAWSON AI runtime

- Added the official NEW PAWSON AI runtime.
- Preserved legacy web research as a migration acceptance baseline.
- Kept both paths temporarily while capabilities moved through real acceptance.

### September 4 | Pluggable expert packages

- Completed official runtime integration.
- Defined the pluggable expert architecture and persona-package template.
- Added task-scoped expert centers.
- Registered bundled expert Skills.
- Added the first visual-diagnosis package, Lingjing.
- Persisted task capabilities across restored conversations.
- Established one structure for future business and document experts.

### September 5 | Three expert disciplines and a local profile center

- Added a task-scoped expert collaboration workspace.
- Completed business-analysis and document-delivery expert packages.
- Brought visual, operations, and document methods into one main task.
- Defined and safely persisted a local user profile.
- Added avatar presets, profile editing, and a sidebar personal center.
- Stabilized AI and product workflows and corrected avatar art direction.
- Saved expert-package and current-state handoffs.

### September 6 | First Codex collaboration milestone

- Closed the official runtime, thread recovery, and mid-task steering loop.
- Enabled three expert methods to collaborate within one task.
- Brought business context, image input, and files into one workspace.
- Improved image recovery, tool activity, and diagnostic evidence.
- Passed 2,342 tests across 365 test files.
- Passed TypeScript, desktop, and production builds.
- Details: [From a toolset to an integrated agent workspace](../updates/2026-09-06.en.md).

<a id="day-2026-09-07"></a>

### September 7 | Three architecture boundaries converged

- Unified task interaction around one runtime truth.
- Made trusted business context a user-controlled read-only input.
- Limited runtime observability to bounded safe metadata.
- Removed page navigation, cross-feature prefilling, and internal action cards after hands-on review.
- Shifted from large core rewrites to small acceptance steps and defect fixes.
- Passed 2,389 tests across 373 files and the full production build.
- Details: [Three architecture boundaries converged](../updates/2026-09-07.en.md).

<a id="day-2026-09-08"></a>

### September 8 | First general AI gateway path

- Retired the previous multi-provider capability router while preserving necessary compatibility data.
- Added a versioned, provider-neutral capability contract.
- Added least-privilege short-lived signed access and public verification boundaries.
- Reused one gateway contract for the desktop Agent, text, image generation, and image editing.
- Kept long-lived provider secrets out of the desktop UI, ordinary logs, and control-center responses.
- Accepted the first live Qwen text path and consumer authorization.
- Details: [The general AI gateway completed its first path](../updates/2026-09-08.en.md).

<a id="latest"></a>

<a id="day-2026-09-09"></a>

### September 9 | Agent capability restoration and the 2.0 release

- Unified the desktop, control center, reports, and collection extension as PAWSON AI Platform 2.0.
- Added a versioned model catalog and conversation-level model selection.
- Issued short-lived enterprise model pools without storing long-lived provider credentials on the desktop.
- Restored web search, public-page reading, and clickable sources.
- Restored expert identity, the global page assistant, and structured file delivery.
- Retired the legacy Agent runtime, local provider direct access, and old data path.
- Isolated 2.0 data while preserving account, credit, and update compatibility.
- Details: [PAWSON AI Platform entered the 2.0 stage](../updates/2026-09-09.en.md).

## Recording principles

This timeline contains only claims supported by commits, checkpoints, tests, builds, real files, or hands-on acceptance. Dates without commits are omitted. Plans, drafts, and UI messages are not rewritten as completion. Private source, full architecture, internal addresses, credentials, customer data, and reproducible implementation remain outside the public record.


