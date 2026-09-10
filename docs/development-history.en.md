# Development Story: From Product-Image Tools to a Local-First AI Workspace

[简体中文](development-history.md) · **English**

> This is a living development journal. Last updated: September 10, 2026.

> 📅 [View the complete history for every active development day](daily-development-history.en.md#latest) · 🚀 [Read the latest update](../updates/2026-09-10.en.md)

PAWSON AI was not completed from one fixed blueprint. It took shape through real deliveries, recovery work, product tradeoffs, and repeated verification. Each phase addressed problems exposed by the previous one and changed what the next phase needed to solve.

This story explains the decisions and outcomes without publishing private source code, full architecture, internal APIs, provider configuration, or security implementation.

## The evolving product line

```text
Product-image production
    ↓
Unified production workspace
    ↓
Operations, data, and knowledge foundation
    ↓
PAWSON Agent MVP
    ↓
Official runtime, experts, and pluggable capabilities
    ↓
PAWSON AI Platform 2.0
    ↓
Commercial access and request-level verification (current)
```

This was not a predetermined feature checklist. Major changes came from concrete friction: results could not continue into another tool, restored tasks lost context, an agent could answer but could not deliver files, or model selection had no clear relationship to a conversation. The product moved forward only after each layer became more reliable.

## The beginning: make product-image production actually work

The first problem was practical. Cross-border product content required constant switching between generation, background removal, cropping, upscaling, mockups, and export. Individual AI features were available, but moving assets, repeating parameters, losing outputs, and verifying whether a task truly succeeded consumed the real time.

By July 25, the early Windows build could handle text-to-image and reference-image workflows, local background removal, precise cropping, upscaling, and product mockups. Both installer and portable delivery artifacts were produced.

This phase established a principle that still governs the project: a UI success state is not proof of completion. Output files must exist, dimensions and formats must be verifiable, failure must preserve valid results, and high-risk output must retain a place for human review.

![Early pattern variation comparison](../screenshots/2026-07-pattern-variation-comparison.png)

> July 2026: the pattern-variation screen evolved from an early result layout into a workspace that clearly separates task parameters, the source image, and candidate results. All visible artwork is test material.

![Local background removal](../screenshots/2026-07-background-removal.png)

> A local background-removal test with transparent output, original-image comparison, download, and manual refinement available together.

![Product mockup workflow](../screenshots/2026-07-product-mockup.png)

> An early product-mockup workspace for positioning, scale, opacity, and export format.

## July 27–28: from local tools to a commercial client

Once the tools could deliver files, a different set of questions appeared: accounts, devices, plans, credits, desktop updates, and payment verification.

The product added a control-center foundation, account and device boundaries, verified payment configuration, provider capability discovery, and desktop release management. Version 1.0.6 then corrected how packaged clients connected to cloud control capabilities.

An early manual-payment route was deliberately removed because it could not provide authoritative settlement evidence. The product moved toward server-verified payment results rather than treating a screenshot or front-end polling state as proof that funds had settled.

## July 30–August 2: isolated tools could not remain isolated

As image features multiplied, users could lose track of which image belonged to which task and how a generated result should continue into cropping, background removal, or mockups.

The next iteration unified task selection, production steps, result presentation, and follow-up processing. It also addressed practical failure cases: rejected provider requests no longer retried blindly, restoring a task did not charge again, duplicate clicks did not create duplicate operations, and connection recovery triggered state reconciliation.

The workspace then moved toward a project-centered model. Assets, parameters, intermediate state, and outputs needed to belong to a recoverable project instead of a temporary page.

## August 4: prove the offline workflow first

Cross-border collection, content preparation, and platform actions were separated into modules that could be tested without a real store account. The offline workflow and UI contracts passed, while live login, selectors, draft saving, and publishing remained explicit manual acceptance items.

This became a lasting documentation rule: implementation, offline verification, and live business acceptance are three different claims.

## August 3–20: expand from production pages into an operations workspace

Product content is only one part of operating a business. Teams still need to understand which products deserve investment, what changed in advertising or refunds, how findings become actions, and how completed actions are reviewed.

PAWSON began to form cross-border operations workspaces, a report center, task views, and a global assistant. A report-delivery milestone arrived on August 12, followed by another stable checkpoint before product-detail work began.

The hard problems were no longer limited to choosing a model. Recommendations needed trusted data, facts had to stay separate from inference, long-running work needed durable context, and transport failures needed recoverable states.

## August 21: the Agent MVP became the new product line

By August 21, the PAWSON Agent MVP had a stable baseline for conversations, task state, professional capability selection, and basic recovery. The product started moving from “many tools with AI” toward “one agent workspace that can use many tools.”

![Agent prototype sign-in screen](../screenshots/2026-08-agent-login.png)

> The August 18 agent prototype still used the PAWSON AIGC identity and focused on connecting product-visual work with the agent workspace.

The transition exposed another risk: an agent that produces polished text but cannot verify files, wait for approval, preserve task state, or recover from failure cannot carry real work. Observability, interruption, recovery, and evidence became primary requirements.

## August 22–26: data, knowledge, and collection became trusted context

The next phase established multitask foundations, web collection, data assets, and knowledge workflows. Collection results gained provenance and lifecycle state instead of remaining temporary downloads.

By August 26, the collection hub and traffic-analysis surfaces were integrated into the product. Data assets could feed knowledge and operations workflows, while product-detail generation started becoming an editable project rather than a one-shot output.

The key lesson was simple: data entering the product does not make it trustworthy. Source, time range, and processing state must remain visible. Missing context should produce a clear limitation instead of a plausible answer assembled from stale conversation history.

## August 27–30: one workspace, recoverable projects, and expert methods

The end of August brought workspace consolidation, an expert-creation flow, a recoverable product-detail library, and a global assistant.

Product-detail projects could be saved, copied, imported, exported, restored, and continued. The global assistant could understand the current page while leaving high-impact actions under user control. Specialized visual, operations, and document methods began replacing one ever-growing generic prompt.

The product decision was to treat expertise as maintained methods with clear boundaries, not as decorative role names or fictional employees.

## September 1: the agent started handling real work

The agent gained controlled command execution, long-running task state, durable file outputs, office-document capabilities, and external Skill discovery.

Three requirements had to advance together: commands needed permission boundaries, interruptions needed to preserve valid work, and generated files needed existence checks. A result card or cached filename could not count as a delivered artifact.

## September 2–6: official runtime and the integrated agent milestone

NEW PAWSON AI adopted the official agent runtime and developed conversation restoration, mid-task steering, stopping, tool activity, errors, image input, and file delivery.

Visual diagnosis, business analysis, and document delivery became three maintained expert disciplines inside the same workspace.

| Lingjing · Visual diagnosis | Guheng · Business analysis | Jianning · Document delivery |
| --- | --- | --- |
| <img src="../screenshots/expert-visual.webp" width="180" alt="Visual diagnosis expert"> | <img src="../screenshots/expert-operations.webp" width="180" alt="Business analysis expert"> | <img src="../screenshots/expert-document.webp" width="180" alt="Document delivery expert"> |

On September 6, these elements formed a clear milestone: PAWSON had moved beyond a collection of tools and gained a unified agent entry point, business context, professional methods, controlled execution, and file delivery. The verification baseline contained 365 test files and 2,342 passing tests, with production builds passing as well.

## September 7: three architecture boundaries converged

After the milestone, the project stopped expanding the core and unified task interaction, trusted business context, and runtime observability and recovery. Start, steering, approval, stall, stop, and recovery returned to one runtime truth. Business data entered the current task only as a user-controlled read-only input, and diagnostics retained only bounded safe metadata.

Hands-on review led to removing Agent-driven page navigation, cross-feature prompt prefilling, and internal action cards. Navigation remained under user control. The full production build and all 2,389 tests across 373 files passed, moving the project into smaller acceptance steps and defect fixes. [Read the complete entry](../updates/2026-09-07.en.md).

## September 8: the first general AI gateway path

After retiring the previous multi-provider router, the project established a provider-neutral versioned capability contract, least-privilege short-lived access, and the first desktop Agent gateway path. Text, image generation, image editing, and product details began sharing one capability catalog, while long-lived provider secrets stayed out of the desktop UI, ordinary logs, and control-center responses.

Model content went directly to the AI gateway, while the control center handled only identity eligibility, capabilities, and short-lived access. The first live Qwen text path and consumer authorization passed hands-on acceptance. Trusted commercial usage reconciliation remained incomplete, so a client result was not described as successful billing. [Read the complete entry](../updates/2026-09-08.en.md).

## September 9: Agent capability restoration and the 2.0 stage

Model selection became conversation-specific. Web search, public-page reading, clickable sources, expert identity, the global assistant, and structured file delivery returned through the new Agent path. The legacy Agent runtime, local provider direct access, and old data path retired from the active product.

That day, the desktop product became PAWSON AI Platform 2.0, unifying the desktop client, control center, reports, and collection extension under one brand while preserving account, credit, local-data, and update compatibility.

![PAWSON AI Platform 2.0 sign-in screen](../screenshots/2026-09-platform-login.png)

> The 2.0 message expands from product-visual production into one workspace for business intelligence, expert collaboration, and content creation.

## September 10: test the smallest commercial-access loop

The P0 probe used the pinned local runtime and a loopback fake upstream. Of 16 final cases, 15 passed and one failed. Text, a harmless tool call, the tool result, and follow-up text completed successfully. The probe also observed request counts and covered identity fields, rate limiting, credential expiry, stream failure, missing usage, and user cancellation.

The failed case exposed an important boundary: a local task entering an interrupted state did not prove that the upstream connection had closed promptly. A separate explicit-abort prototype closed the matching connection, but it has not been integrated into the daily agent path. The outcome remains 15/16 rather than being rewritten as a complete P0 success.

No paid model was called, no database was migrated, and no production service was deployed. Real gateway behavior, provider-side acceptance and metering, and multi-tenant concurrency remain future verification work.

## How this story will continue

Each verified milestone will be added to this document and receive a dated entry under `updates/`. New entries follow four rules:

1. Only completed or verified work is presented as a result.
2. Product direction, code baselines, and live-service acceptance remain separate.
3. Important tradeoffs and failures are recorded without exposing reproducible core implementation.
4. Credentials, customer data, internal addresses, full architecture, and security configuration remain private.

The next chapter will follow new evidence from the request-level access work.
