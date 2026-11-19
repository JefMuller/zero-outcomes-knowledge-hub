The Accelearted response Blue
> Using single use cases to verify a solid foundation for initial success and definition.

## Source and intended use

- Source: user-supplied image titled **Accelerated Response Blueprint**, labelled **Single Slide View**, slide 3.
- Scope: this document converts the supplied slide only; it does not represent an extraction of the full presentation.
- Language: English, matching the source and intended technical documentation corpus.
- Sections 1–8 preserve the blueprint content with light editorial normalization. Sections 9–13 are added instructions for generating an implementation guide; they are not claims from the slide.
- Revision 2: research, release applicability, dependency classification, and execution-readiness rules strengthened following review of an initial generated guide. No new product configuration claims have been validated by this revision.
- This is an outcome and sequencing reference. Exact configuration steps must be grounded in documentation for the customer's release and application versions.
- No ServiceNow documentation repository has been connected or inspected for this conversion. Repository URL, branch, documentation coverage, and release applicability remain to be supplied and verified.

## 1. Outcome, scope, and capability bands

Start with one or two service-instance/application use cases, prove the foundations and operational response, then document a repeatable pattern for more services.

The slide groups work into these capability bands:

| Band | Coverage shown on the slide |
| --- | --- |
| Use Case | Selected service-instance/application use case and owners |
| CMDB Health – Service Mapping – Plugins | Data foundations and prerequisites |
| Event Management – AIOps – Change – LEAP – KB – Specialists | Event ingestion, context, and Specialist activation |
| Incident – Major Incident | Incident process refinement and optional major incident process |
| Overall Testing and KPIs | Observation, value measurement, refinement, and progression |

## 2. Phase 1 — Define, Prep, Discover, Map & Populate

### Purpose

Deploy Discovery using top-level scans and/or ACC agents, populate the CMDB for the target scope, and reconcile and assign CI ownership. Stretch goal: build service maps for two or three Tier 1 services. Install all instance prerequisites for the required steps.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P1.1 | Document one or two service-instance (application) use cases and their owners. |
| P1.2 | Install plugins and activate AI Skills. |
| P1.3 | Add CIs to the CMDB through Service Graph Connector and/or Discovery for the defined use-case scope. |
| P1.4 | Create a simple Service Model for the use case, using a tag-based map. |

### Interpretation notes

- The phase description mentions two or three Tier 1 service maps as a stretch goal; the first timeline action scopes one or two use cases. Preserve both statements rather than treating the stretch goal as mandatory initial scope.
- The slide does not identify plugin IDs, AI Skills, roles, licenses, discovery credentials, or connector selection criteria.
- Ownership reconciliation is in the phase description and must remain part of implementation planning even though it has no separate timeline dot.

## 3. Phase 2 — Connection and Correlation

### Purpose

Connect event sources that provide comprehensive event inputs for the use case. Ensure alert grouping and use-case coverage.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P2.1 | Configure Event Management connector(s) to hydrate events into alerts. |
| P2.2 | Review alert groups for enrichment and grouping with Alert Automation. |

### Interpretation notes

The slide supplies no connector-specific configuration, correlation logic, thresholds, CI-binding rules, or test-event procedures. Derive those from verified documentation and the chosen event sources.

## 4. Phase 3 — Add Context and Activate Specialist

### Purpose

Use tools such as LEAP to learn from prior incident data and produce Knowledge Base and Playbook outputs. Use these outputs to add context so the Specialist can function to maximum effect.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P3.1 | Generate knowledge articles (KBs) and playbooks from LEAP opportunities. |
| P3.2 | Add change records for CIs to provide root-cause context. |
| P3.3 | Activate AIOps Specialist for the team. |

The slide marks a demonstration near Specialist activation.

### Gate to Phase 4

The slide lists the following readiness items:

- [ ] CI coverage for one service.
- [ ] Incoming events.
- [ ] Knowledge Base for one service.
- [ ] Change record for one service.
- [ ] LEAP activated for KB on one service.
- [ ] Specialist activated for one service.

These are source readiness statements. Define measurable evidence for each before using them as operational acceptance criteria. The slide does not define the required completeness of CI coverage or KB content.

## 5. Phase 4 — Incident Process Refinement

### Purpose

If the current workflow creates incidents for every event, review alert outcomes using the Specialist and reduce incident creation wherever possible. Internal standard operating procedures and reporting may need adjustment.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P4.1 | Review the incident workflow SOP to support alert adoption and reduce incidents. |
| P4.2 | Add or adjust incident-creation Alert Automation respond rules. |
| P4.3 | Configure On Call / SRM team activations, automations, and workflows — optional. |

The slide marks a demonstration near the optional On Call / SRM action.

## 6. Phase 5 — Major Incident Process (optional)

### Purpose

Review and refine standard operating procedures for using alerts and incidents, including how escalation to major incidents occurs.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P5.1 | Configure the Major Incident trigger for P1. |
| P5.2 | Configure On Call team activations, automations, and workflows. |
| P5.3 | Test the Major Incident process. |

### Interpretation notes

- This entire phase is optional.
- “P1” above is the slide's priority designation, distinct from this document's Phase 1 step IDs.
- The slide does not define the priority model, approval policy, or whether the trigger proposes or automatically promotes a major incident. Resolve these using the customer's operating model and release-specific documentation.

## 7. Phase 6 — Observation and Refinement

### Purpose

Allow the service(s) to operate with team engagement to understand the process, identify gaps, and improve the pattern so it can be repeated with more services.

### Ordered steps

| ID | Blueprint action |
| --- | --- |
| P6.1 | Observe and measure value with users. |
| P6.2 | Refine and document a repeatable process for more services. |

The slide marks a demonstration near observation and measurement.

### Gate to Self Healing

Preserve the slide's thresholds exactly:

| Metric wording on slide | Threshold on slide | Definition still required |
| --- | --- | --- |
| False grouping | <15% | Definition of incorrect grouping, denominator, sampling, and adjudication |
| False escalation | <20% | Definition of incorrect escalation, denominator, and adjudication |
| Summaries | >80% | What is measured: coverage, completion, quality, or another property |
| Rated “useful” | >60% | Which output is rated, rating scale, respondents, and denominator |
| Triage accuracy | >75% | Ground truth, scoring method, and denominator |
| Rated “actionable” | >70% | Which output is rated, rating scale, respondents, and denominator |

The slide does not define an observation window, minimum sample size, or who signs off. Do not silently supply these as source facts. Passing this gate does not itself specify or authorize self-healing configuration; that implementation is outside this slide.

## 8. Terminology and source ambiguities

| Term | Meaning or treatment for the implementation guide |
| --- | --- |
| CI | Configuration Item |
| CMDB | Configuration Management Database |
| KB | Knowledge Base / knowledge article, depending on context; confirm which record or capability the source step requires |
| SOP | Standard Operating Procedure |
| ACC | Agent Client Collector; verify the specific agent components required for the target release |
| Service Graph Connector | Connector-based CMDB population option named on the slide |
| Discovery | Discovery-based CMDB population option named on the slide |
| Service Model / tag-based map | Source terminology; verify exact target record types and mapping workflow |
| Alert Automation | Source terminology; verify the supported features, UI labels, and rule types |
| AIOps Specialist | Source capability name; verify availability, prerequisites, entitlement, activation, and supported behavior |
| AI Skills | Unspecified skills on the slide; identify the required skills through documentation |
| LEAP | Source capability name; expansion, availability, and exact workflow are not supplied |
| SRM | Source abbreviation; expansion and intended capability are not supplied |
| On Call | Source wording; verify the official application name and supported workflow |

---

## 9. Added guidance — Documentation corpus and provenance

Use the blueprint to define the intended outcome and phase order. Use authoritative, applicable ServiceNow documentation to establish how each action is implemented.

Before generating executable instructions, record:

- Target platform release and patch.
- Installed application / Store application versions.
- Relevant entitlements, available plugins, user roles, and environment type.
- Selected use case, service owner, technical owner, and event source(s).
- Current CMDB, discovery, mapping, alert, incident, and on-call maturity.
- Exact documentation repository URL, owner, branch or tag, and commit SHA.
- Repository coverage: which products and releases it actually documents.
- Approved official documentation sources for topics absent from the repository.

Do not assume a repository contains the complete ServiceNow product documentation or is authoritative solely because its name mentions ServiceNow. Verify publisher, purpose, release coverage, and source provenance. Keep examples and sample code distinct from supported product instructions.

For each implementation claim, cite a repository path and section at a pinned commit, or an official documentation URL and applicable release. Label every addition as one of:

1. **Blueprint requirement** — traceable to a step or gate above.
2. **Documented prerequisite / procedure** — supported by an applicable source.
3. **Recommended practice** — an explicit recommendation with rationale.
4. **Customer decision** — requires a local operating-model choice.
5. **Unresolved** — evidence is missing or conflicting.

If documentation conflicts with the slide, describe the conflict and propose a documented route that preserves the outcome. Do not silently rewrite the blueprint or fabricate a configuration path.

## 10. Added guidance — Required implementation-guide structure

Write for a first-time implementer. Explain unfamiliar terms at first use and use one action per numbered instruction. Do not rely on “configure as appropriate.”

For each step, include:

| Field | Required content |
| --- | --- |
| Step ID and blueprint mapping | Stable ID and link to P1.1–P6.2 or a named gate |
| Objective | Expected observable result and why it matters |
| Applicability | Platform release, application version, and relevant conditions |
| Dependencies | Earlier steps that must pass; branch conditions and optionality |
| Responsible person | Required role and owner; identify customer decisions |
| Prerequisites | Entitlements, plugins, access, connectivity, data, and approvals when applicable |
| Inputs | Exact information the user must collect; use labelled placeholders |
| Procedure | Verified navigation, fields, values, and save/activation actions |
| Expected result | What the user should see after completing the action |
| Verification | Concrete test with pass/fail criteria and evidence to retain |
| Troubleshooting | Documented symptoms, checks, and recovery actions |
| Reversal | How to undo the change where supported; identify irreversible actions |
| Sources | Precise citations supporting the procedure and prerequisites |
| Open issues | Unsupported details, questions, and blockers |

Do not invent plugin identifiers, roles, tables, properties, menu paths, APIs, scripts, ports, AI activation requirements, or default values. If a detail is not verified, label it unresolved and withhold the dependent executable instruction.

Keep the six-phase narrative while exposing prerequisite dependencies. If a documented prerequisite must occur earlier than its capability appears on the slide, add a clearly labelled prerequisite step and explain the dependency.

## 11. Added guidance — Validation and completion

The generated guide should include:

- A readiness checklist before configuration begins.
- A dependency-aware sequence with mandatory, conditional, and optional steps clearly marked.
- A small, representative service use case and controlled test inputs; distinguish example data from required values.
- End-to-end evidence from event receipt through alerts, grouping, CI/service context, Specialist output, and incident handling as applicable.
- Explicit validation of the six Phase 4 gate items.
- A separate branch for the optional Major Incident phase.
- An observation plan defining baselines, metric formulas, sample sizes, time window, and accountable reviewers. Treat these as proposed definitions until agreed.
- The original strict KPI inequalities, including the unresolved meaning of “>80% summaries.”
- A repeatable rollout checklist for additional services, with known limitations and unresolved blockers.

Guide completeness and implementation completion are separate. A complete guide contains source-backed procedures for every selected mandatory step, with customer decisions and any genuine blockers visible. An implementation is complete only when its required tests and gates have passed with recorded evidence. Apply the research and readiness classifications in section 13; an unread page is not an implementation blocker. Do not claim readiness or successful implementation merely because a guide has been written.

## 12. Copy-ready prompt for Claude

```text
Use accelerated_response_blueprint.md as the outcome and sequencing reference.
Use the connected ServiceNow documentation corpus as implementation evidence.
Apply all research and quality rules in section 13 before finalizing the guide.

Create a detailed implementation guide that a first-time ServiceNow implementer
can follow, from prerequisites through validation and operational handover.

First inventory the available documentation and report its publisher, repository
URL, branch/tag, commit, product coverage, and release applicability. Do not assume
the repository is the complete ServiceNow product documentation. Identify gaps.

Extract any known target release, application versions, entitlements, use case,
event sources, access, and current configuration from the supplied materials.
Ask only for missing information that blocks a specific decision. In parallel,
produce the phase outline, dependency map, and documentation coverage matrix.

Preserve all six phases, the optional nature of Phase 5 and Phase 4's On Call / SRM
step, every Phase 4 gate item, and every Self Healing gate threshold. Preserve the
distinction between the initial one or two use cases and the stretch goal of maps
for two or three Tier 1 services.

Map each guide step to a blueprint ID. Add documented prerequisites where needed,
but label additions and explain any sequencing change. For every step use the
fields in section 10. Include exact navigation and field values only when verified
for the target version. Cite the relevant source at the point of use, using a
pinned repository path and section or an official documentation URL and release.

Separate blueprint requirements, documented procedures, recommendations, customer
decisions, and unresolved items. Never invent missing plugin IDs, roles, tables,
properties, APIs, scripts, menu paths, entitlements, or activation requirements.
Block dependent executable steps when their prerequisites cannot be verified.

Define validation checks, expected results, troubleshooting, supported reversal,
and evidence to retain. Propose explicit metric definitions and observation
criteria where the slide is ambiguous, but do not present proposals as approved
requirements. Self-healing implementation is outside the supplied blueprint.

Deliver the guide in Markdown with: context and assumptions; source inventory;
readiness checklist; documentation coverage matrix; dependency-aware numbered
steps by phase; gate validation; optional major incident branch; measurement plan;
repeatable rollout checklist; and a consolidated list of unresolved questions.
Include separate research and execution-readiness statuses, a claim-to-source
evidence register, branch-specific tests, and a correction log for revisions.
Retrieve identified but unread pages before declaring documentation unavailable.
Resolve release discrepancies with source passages and repository metadata;
do not treat earlier generated guides as evidence. Separate technical dependencies
from rollout order and keep connector-specific prerequisites conditional.
Ask only for customer-specific facts unavailable in the materials. Continue all
independent research while those answers are pending. If tools become unavailable,
report the access limitation, preserve verified findings, and list exact retrieval
targets for resumption; do not claim missing functionality or completed research.
Do not stop solely because the conversation is long. If a context limit prevents
completion, provide a resumable checkpoint with completed work and outstanding tasks.
```

## 13. Added guidance — Research discipline and execution readiness

### 13.1 Research status is distinct from implementation readiness

Record research status separately for each step or unresolved claim:

| Research status | Meaning and required next action |
| --- | --- |
| Not yet researched | Relevant evidence has not been read. Retrieve it; do not call this blocked or unsupported. |
| Partially researched | Some evidence is available. Name the unread pages and missing fields, then continue retrieval. |
| Source verified | The relevant full source sections have been read and applicability assessed. This alone does not prove a complete procedure or a successful implementation. |
| Retrieval unavailable | A tool, index, permission, or link prevents access. Record the failed route and exact target; use available authoritative alternatives and continue independent work. |
| Documentation unavailable | Targeted searches and available authoritative routes have been exhausted without adequate evidence. Record search scope, sources checked, date, and remaining uncertainty. This means evidence was not found, not that the capability does not exist. |
| Customer information required | A specific local fact or operating-model decision cannot be obtained from supplied materials. State which decision it affects and continue independent research. |

Use separate execution-readiness labels:

| Readiness | Criteria |
| --- | --- |
| Partial procedure | Required instructions, applicability, prerequisites, or tests remain unresolved. Clearly mark incomplete sections. |
| Execution-ready, not tested | Full applicable procedure retrieved; required fields, dependencies, branch decisions, activation, expected results, and verification instructions documented. Required prerequisites are confirmed, or individually stated as explicit conditions before execution. No essential configuration detail may remain unsupported. |
| Blocked for execution | A named unmet prerequisite, unresolved critical applicability issue, missing customer decision, or essential evidence gap prevents a specific action. Identify the exact dependency and resolution needed. Continue work on unaffected actions. |
| Validated in instance | Recorded test evidence confirms the procedure on a named platform patch and application versions, with test date and reviewer. This does not imply validation on other releases or all customer environments. |

If retaining the label **Executable**, use it only as a synonym for **Execution-ready, not tested**, with the same criteria. Do not mark Specialist activation complete while required task-module configuration is unread, or LEAP setup complete while required installer fields are omitted. A missing documented reversal should be disclosed, not invented; identify whether it prevents safe execution for the selected action.

### 13.2 Verify applicability and maintain a claim-to-source register

Before presenting release-specific instructions, compare the target platform release and patch, Store application versions, source page release labels, and repository metadata. A branch name is context, not sufficient proof that every page describes that release.

- Investigate discrepancies such as Australia-labelled pages stating a Brazil prerequisite. Retrieve the exact passage and assess whether it describes a minimum platform version, an application dependency, a documentation error, or an unresolved inconsistency. Do not assume the explanation or copy a minimum from a prior generated answer.
- Do not infer different roles solely from a display label versus a technical role ID. Likewise, distinguish an installed component ID from the application or bundle used to install it before declaring release differences.
- If the commit SHA cannot be retrieved, disclose that branch citations are mutable. Retain exact paths, source sections, release labels, and retrieval dates. Do not fabricate a SHA or describe a branch citation as pinned.
- Keep excerpts and search snippets as discovery evidence. Read the full relevant source sections before treating a detailed procedure as verified.
- Do not combine instructions from different releases into one executable procedure without explicit evidence of compatibility. Keep historical comparisons outside the selected execution path.

For every consequential configuration claim, record: claim ID; blueprint step; exact claim; source URL or repository path and section; commit when available; source release; application version; brief supporting passage or faithful paraphrase; retrieval date; applicability assessment; and unresolved discrepancy. Prior AI output and this blueprint's added guidance are not product-documentation evidence.

Minimum versions, plugin IDs, roles, provider availability, region restrictions, domain-separation limits, cardinality limits, UI paths, defaults, and system properties all require this traceability. Do not convert a proposed customer approval process into a documented product prerequisite.

### 13.3 Separate dependencies, rollout sequence, and conditional branches

Keep the six-phase blueprint order as the recommended rollout narrative. For each dependency edge, identify its type:

- **Technical prerequisite:** supported by a cited product requirement.
- **Blueprint gate:** required by a named readiness item in the slide.
- **Recommended rollout order:** useful sequencing, with rationale; not claimed as a product constraint.
- **Customer policy:** a locally agreed rule, with owner.
- **Conditional dependency:** applies only to a selected connector, feature, module, or branch; state its condition.

Do not infer a technical dependency from the slide's timeline. In particular, do not assume LEAP requires completed alert grouping or service mapping, or that event ingestion requires complete CMDB population. Investigate the actual requirements, including the distinction between event receipt, alert creation, CI binding, and service-impact analysis. Absence of a requirement on one page is not proof of independence.

Maintain a prerequisite matrix with columns: capability; plugin/application; version; role; condition; supporting source; target-instance confirmation. Connector-specific plugins belong only in the matching connector branch. Do not make an Azure or AWS metrics requirement universal. Distinguish service families, generated service instances, and the blueprint's outcome of a usable service model; do not assume they are interchangeable objects.

### 13.4 Close research gaps systematically

Maintain a retrieval backlog mapped to blueprint IDs. At minimum investigate:

| Step | Required research coverage |
| --- | --- |
| P1.2–P1.3 | Applicable installation procedures; Service Graph Connector, Discovery, and ACC options; identification/reconciliation and ownership for the selected scope |
| P1.4 | Required tags, mapping prerequisites, service families versus service instances, resulting service map, and verification |
| P2.1–P2.2 | Selected connector setup; event-to-alert processing; CI binding; enrichment; grouping; Alert Automation |
| P3.1 | LEAP installation, full installer fields, history/data requirements, activation, generated outputs, and any documented KB creation or promotion workflow |
| P3.2 | Change record configuration, affected-CI relationships, and how the selected Specialist uses change context |
| P3.3 | Onboarding, alert scope, required task modules, testing, activation, deactivation, restrictions, and dashboard metrics |
| P4.2 | Respond automation and applicable classic rules; exact field mapping; duplicate-incident prevention and verification |
| P4.3 / P5.2 | Official meaning of SRM in this context, On Call/team activation requirements, workflows, and tests for selected optional branches |
| P5.1–P5.3 | Major Incident Management activation, trigger conditions, propose/promote behavior, playbook, and branch-specific tests |
| P6.1–P6.2 | Dashboard metric definitions, evidence collection, agreed blueprint KPIs, and repeatable rollout controls |

Use repository navigation, links from retrieved pages, exact-title searches, and available official documentation routes. Log what was actually read. If a search index is unavailable, distinguish indexing/access limitations from missing documentation. Ask the user for customer-specific facts, not to perform research that available tools can complete.

### 13.5 Investigate differences before declaring conflicts

- An overview omitting a feature does not establish that it is unsupported. Specifically research LEAP knowledge-article creation or promotion, application versions, and any separate workflow involved. Preserve the blueprint's KB outcome while marking its implementation route unresolved until substantiated.
- “Updated” or “recommended” does not mean older functionality is deprecated, removed, or unsupported. Verify those lifecycle claims explicitly and distinguish classic alert rules, response automation, and any deprecated subfeature.
- Different configuration routes can be alternatives, overlapping mechanisms, or complementary stages. Establish actual overlap and duplicate-action risks before requiring an exclusive choice.
- Community material may identify search leads but must remain labelled separately from official evidence. Do not insert unverified scripts or examples into executable instructions.

### 13.6 Verify field mappings and test every selected branch

For each field mapping, verify source field meaning, destination field type, reference resolution, transformation, defaults, and expected stored value. **Do not use Alert source → Configuration item** as an example unless an authoritative applicable source explicitly supports the mapping and its resolution logic. A source-system identifier must not be assumed to identify a CI.

Tests must match configured behavior:

- If the selected documented action proposes a major incident, test for the expected candidate state and approval path. If it promotes directly, test for the expected major incident state. Verify exact state and record behavior from applicable documentation.
- For automatic incident creation, test matching and non-matching alerts, required field population, waiting behavior, and overlapping automation. For manual execution, include the required operator action; a matching alert alone must not imply automatic creation.
- Verify grouping and maintenance conditions according to the configured branch. State expected results separately for each case.
- Do not present a timing property as a duplicate-incident fix without evidence of causality. Check overlapping rules/subflows and execution records; cite the supported diagnostic procedure.
- Label proposed test criteria separately from documented behavior and retain actual results separately from expectations.

### 13.7 Deliverable review and continuity

Before delivering a revised implementation guide, confirm:

- [ ] All six phases, stable step IDs, optionality, Phase 4 gate items, and strict KPI thresholds remain intact.
- [ ] Research gaps and execution blockers have separate statuses and next actions.
- [ ] Every execution-ready procedure has complete required fields, applicable prerequisites, activation steps, and branch-specific verification.
- [ ] Release-specific claims and dependencies have traceable evidence; conditional requirements remain conditional.
- [ ] Unsupported mappings and unverified product claims have been removed from execution instructions or clearly marked unresolved.
- [ ] A short correction log identifies each changed claim, its replacement, rationale, and supporting source where available.
- [ ] Remaining customer questions identify exactly which actions depend on their answers.

Continue all research independent of pending customer answers. Do not stop solely because the conversation is long. If tools or context limits genuinely prevent completion, provide a resumable checkpoint containing the current draft, verified source register, unread exact paths/titles, failed access routes, pending decisions, and next actions. Do not claim completion or imply a new chat will necessarily restore unavailable tools.
