<!--
Sync Impact Report:
Version change: 0.0.0 → 1.0.0
Modified principles:
  - PROJECT_NAME → Calculator
  - PRINCIPLE_1_NAME → I. Library-First
  - PRINCIPLE_1_DESCRIPTION → Every feature starts as a standalone library...
  - PRINCIPLE_2_NAME → II. CLI Interface
  - PRINCIPLE_2_DESCRIPTION → Every library exposes functionality via CLI...
  - PRINCIPLE_3_NAME → III. Test-First (NON-NEGOTIABLE)
  - PRINCIPLE_3_DESCRIPTION → TDD mandatory: Tests written...
  - PRINCIPLE_4_NAME → IV. Integration Testing
  - PRINCIPLE_4_DESCRIPTION → Focus areas requiring integration tests...
  - PRINCIPLE_5_NAME → V. Observability & Simplicity
  - PRINCIPLE_5_DESCRIPTION → Text I/O ensures debuggability...
  - SECTION_2_NAME → Development Workflow
  - SECTION_2_CONTENT → Code review requirements...
  - SECTION_3_NAME → Quality Gates
  - SECTION_3_CONTENT → All code must pass static analysis...
  - GOVERNANCE_RULES → This Constitution supersedes all other practices...
  - CONSTITUTION_VERSION → 1.0.0
  - RATIFICATION_DATE → 2025-12-03
  - LAST_AMENDED_DATE → 2025-12-03
Added sections:
  - Development Workflow
  - Quality Gates
Removed sections:
  - [PRINCIPLE_6_NAME] and [PRINCIPLE__DESCRIPTION] (placeholder removed as not used)
Templates requiring updates:
  - .specify/templates/plan-template.md ✅ updated
  - .specify/templates/spec-template.md ✅ updated
  - .specify/templates/tasks-template.md ✅ updated
  - .specify/templates/commands/sp.checklist.md ✅ updated
  - .specify/templates/commands/sp.constitution.md ✅ updated
  - .specify/templates/commands/sp.adr.md ✅ updated
  - .specify/templates/commands/sp.clarify.md ✅ updated
  - .specify/templates/commands/sp.git.commit_pr.md ✅ updated
  - .specify/templates/commands/sp.implement.md ✅ updated
  - .specify/templates/commands/sp.analyze.md ✅ updated
  - .specify/templates/commands/sp.plan.md ✅ updated
  - .specify/templates/commands/sp.phr.md ✅ updated
  - .specify/templates/commands/sp.specify.md ✅ updated
  - .specify/templates/commands/sp.tasks.md ✅ updated
Follow-up TODOs: none
-->
# Calculator Constitution
<!-- Defines the foundational principles and guidelines for the Calculator project. -->

## Core Principles

### I. Library-First
<!-- Example: I. Library-First -->
Every feature starts as a standalone library; Libraries must be self-contained, independently testable, documented; Clear purpose required - no organizational-only libraries.
<!-- Example: Every feature starts as a standalone library; Libraries must be self-contained, independently testable, documented; Clear purpose required - no organizational-only libraries -->

### II. CLI Interface
<!-- Example: II. CLI Interface -->
Every library exposes functionality via CLI; Text in/out protocol: stdin/args → stdout, errors → stderr; Support JSON + human-readable formats.
<!-- Example: Every library exposes functionality via CLI; Text in/out protocol: stdin/args → stdout, errors → stderr; Support JSON + human-readable formats -->

### III. Test-First (NON-NEGOTIABLE)
<!-- Example: III. Test-First (NON-NEGOTIABLE) -->
TDD mandatory: Tests written → User approved → Tests fail → Then implement; Red-Green-Refactor cycle strictly enforced.
<!-- Example: TDD mandatory: Tests written → User approved → Tests fail → Then implement; Red-Green-Refactor cycle strictly enforced -->

### IV. Integration Testing
<!-- Example: IV. Integration Testing -->
Focus areas requiring integration tests: New library contract tests, Contract changes, Inter-service communication, Shared schemas.
<!-- Example: Focus areas requiring integration tests: New library contract tests, Contract changes, Inter-service communication, Shared schemas -->

### V. Observability & Simplicity
<!-- Example: V. Observability, VI. Versioning & Breaking Changes, VII. Simplicity -->
Text I/O ensures debuggability; Structured logging required; Start simple, YAGNI principles.
<!-- Example: Text I/O ensures debuggability; Structured logging required; Or: MAJOR.MINOR.BUILD format; Or: Start simple, YAGNI principles -->


## Development Workflow
<!-- Example: Additional Constraints, Security Requirements, Performance Standards, etc. -->

Code review requirements: all code changes require at least one approving review. Automated testing gates must pass before merging. Deployment approval process requires explicit sign-off from tech lead.
<!-- Example: Technology stack requirements, compliance standards, deployment policies, etc. -->

## Quality Gates
<!-- Example: Development Workflow, Review Process, Quality Gates, etc. -->

All code must pass static analysis and linting checks. Unit test coverage must be at least 80%. Integration tests must pass for all new features and major changes.
<!-- Example: Code review requirements, testing gates, deployment approval process, etc. -->

## Governance
<!-- Example: Constitution supersedes all other practices; Amendments require documentation, approval, migration plan -->

This Constitution supersedes all other practices. Amendments require formal documentation, approval by the tech lead, and a clear migration plan for affected systems. All Pull Requests and code reviews must verify compliance with these principles. Unjustified complexity is prohibited.
<!-- Example: All PRs/reviews must verify compliance; Complexity must be justified; Use [GUIDANCE_FILE] for runtime development guidance -->

**Version**: 1.0.0 | **Ratified**: 2025-12-03 | **Last Amended**: 2025-12-03
<!-- Example: Version: 2.1.1 | Ratified: 2025-06-13 | Last Amended: 2025-07-16 -->