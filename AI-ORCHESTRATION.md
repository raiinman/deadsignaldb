# Multi-Model Working Protocol

## Purpose

Dead Signal DB may use several AI systems as a deliberate team. The team is not a vote. It is a pipeline in which different models contribute different strengths, while one orchestrator preserves the product thesis, tracks decisions, and owns integration.

The human owner remains the final authority for taste, priorities, account access, publishing, and deployment.

## Roles

### Orchestrator: GPT-5.6 Luna in Codex

The orchestrator owns the brief, repository context, constraints, research framing, model routing, synthesis, implementation, testing, and final recommendation.

Luna is the default for routine planning, document maintenance, repository inspection, small-to-medium code changes, and high-volume iteration. It is also the continuity layer: other models may suggest ideas, but the orchestrator decides what becomes part of Dead Signal DB.

For work that is unusually ambiguous, brand-defining, technically risky, or expensive to reverse, the orchestrator should escalate to a higher reasoning tier when the environment makes one available. Current OpenAI guidance describes GPT-5.6 Luna as optimized for cost-sensitive workloads, GPT-5.6 Terra as the balance tier, and GPT-5.6 Sol as the flagship for complex professional work. This is a routing rule, not a claim that every task needs the most expensive model. [Official OpenAI model guidance](https://developers.openai.com/api/docs/models)

### Claude

Use Claude for:

- brand strategy and naming alternatives
- long-form synthesis and critique
- information architecture
- voice, positioning, and editorial systems
- identifying ambiguity or contradictions in written plans

Claude is a challenger and strategist. It should receive a bounded question and explicit evaluation criteria, not an invitation to redesign the entire product without constraints.

### Gemini

Use Gemini for:

- visual and multimodal analysis
- screenshots, reference sites, and image direction
- visual interaction concepts
- comparative web research
- generating alternative experience directions

Gemini is especially useful when the question depends on seeing a page, image, animation, layout, or visual system. Its output should still be checked for factual accuracy and feasibility.

### Human owner

The owner decides what the brand should mean, what is worth building, what may be published, and which external accounts or services may be used. The owner supplies model outputs to the orchestrator when no direct connector exists.

## Model-routing matrix

| Task | Default | Add a second opinion when | Escalate reasoning when |
|---|---|---|---|
| Small copy or documentation edit | GPT-5.6 Luna | wording changes brand meaning | the change affects the core positioning |
| Repository inspection or ordinary implementation | GPT-5.6 Luna | architecture has competing options | the change can break deployment or data integrity |
| Brand positioning | Claude + GPT-5.6 Luna | always compare distinct directions | the decision defines the long-term parent identity |
| Visual identity or interaction direction | Gemini + Claude | whenever visual references are involved | the choice creates major implementation debt |
| Website information architecture | Claude + GPT-5.6 Luna | when project types differ substantially | navigation will constrain future projects |
| Web research | Gemini or GPT-5.6 Luna with web search | when sources disagree | claims affect strategy, legal, safety, or money |
| Accessibility and UX review | GPT-5.6 Luna + Claude | after major interface work | interaction is novel or heavily animated |
| Complex frontend architecture | GPT-5.6 Terra or Sol if available | obtain a second technical critique | state, performance, or deployment risk is high |
| Final code integration and tests | GPT-5.6 Luna | request targeted review from Claude/Gemini | failure would damage a live product |

## Escalation rules

The orchestrator should increase reasoning effort or move from Luna to Terra/Sol when at least one condition is true:

1. The decision is difficult to reverse after launch.
2. The problem has several interacting constraints.
3. A first pass produced unresolved contradictions.
4. The work touches deployment, authentication, data migration, security, payments, or public claims.
5. The output will become a foundational document or shared architecture.
6. The orchestrator is uncertain whether the proposed solution satisfies the user’s actual intent.

Stay on Luna when the task is mechanical, well specified, reversible, or primarily a formatting/build step. Higher tier is for uncertainty and consequence, not prestige.

If a higher tier is unavailable in the current environment, the orchestrator should say so and compensate with narrower scope, additional verification, or a second-model critique.

## Standard working loop

1. **Frame:** write the decision question, context, constraints, and success criteria.
2. **Route:** choose the least expensive model that can answer well; add specialists only when they provide a distinct capability.
3. **Prompt:** give every collaborator the same relevant source context and a role-specific assignment.
4. **Collect:** preserve responses without blending them prematurely.
5. **Compare:** separate agreement, disagreement, evidence, preference, and unsupported speculation.
6. **Decide:** make one recommendation, record rejected alternatives, and identify the reason.
7. **Implement:** change the repository only after the decision is clear.
8. **Verify:** test the result against the brief, technical constraints, accessibility, and real user intent.
9. **Record:** update the relevant planning document when the decision changes the system.

## Prompt contract

Every external model request should include:

- the exact decision to make
- the project context
- known constraints
- what the model owns
- what it must not decide
- the format of the response
- evaluation criteria
- a request to label assumptions and uncertainty

Example:

> You are the brand-strategy reviewer for Dead Signal DB. Evaluate three possible parent-brand directions. The brand must support games, software, tools, and experiments; projects may have independent visual identities; Wakeframe and Once Human already exist. Do not design the page or choose typography. Return: positioning, promise, vocabulary, risks, and a score for distinctiveness, flexibility, clarity, and implementation cost. Label assumptions separately from observations.

## Disagreement protocol

When models disagree, do not average the answers. Classify the disagreement:

- **Fact disagreement:** research or verify the claim.
- **Interpretation disagreement:** state which interpretation better fits the brief.
- **Taste disagreement:** preserve alternatives for the owner to choose.
- **Scope disagreement:** narrow the question before continuing.
- **Capability disagreement:** test a small prototype or inspect the repository.

Model consensus is not evidence. A confident answer is not a verified answer.

## Decision record

For any foundational decision, record:

```text
Decision:
Date:
Question:
Context:
Options considered:
Chosen direction:
Why:
Rejected alternatives:
Risks:
Revisit trigger:
```

## Guardrails

- Do not share credentials, tokens, private server access, or secrets.
- Do not allow a model to push, deploy, purchase, message, or change accounts without explicit human authorization.
- Do not treat generated copy, research summaries, or visual concepts as facts without checking them.
- Keep external research, model speculation, and repository evidence labeled separately.
- Do not let a specialist silently override `BRAND.md` or `WEBSITE-PLAN.md`.
- Do not involve more models simply because a decision feels uncomfortable; escalate only when the added perspective changes confidence or coverage.

## Current routing decision

For the next Dead Signal DB phase:

- Use GPT-5.6 Luna for repository work, synthesis, documentation, and normal implementation.
- Use Claude for independent brand and information-architecture critique.
- Use Gemini for visual references, screenshots, and interaction exploration.
- Escalate the orchestrator to GPT-5.6 Terra or GPT-5.6 Sol for the final brand architecture decision or any high-consequence technical design, if available.

No external model should be consulted until the current planning documents have been reviewed and the question is written down precisely.
