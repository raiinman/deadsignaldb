# Multi-Model Working Protocol

## Purpose

Claude and Gemini are optional specialist collaborators. Dead Signal DB decisions remain coherent because one orchestration process frames questions, compares answers, records decisions, and integrates approved work.

## Roles

- **Orchestrator:** defines the question, constraints, acceptance criteria, synthesis, and final implementation.
- **Claude:** brand strategy, information architecture, writing, critique, and long-form reasoning.
- **Gemini:** visual exploration, multimodal analysis, web research, and alternate concepts.
- **Human owner:** final taste, authorization, account access, deployment, and project priorities.

## Working loop

1. Frame one bounded question.
2. Give each model a role-specific prompt and the same source context.
3. Bring the responses back for comparison.
4. Separate agreement, disagreement, evidence, and preference.
5. Make one recommendation or explicitly preserve alternatives.
6. Record the decision before implementation.
7. Review the implementation against the decision record.

## Guardrails

- Do not ask multiple models to independently “design the whole site” without shared criteria.
- Do not treat model agreement as proof.
- Do not let generated ideas silently override the brand foundation.
- Keep external research and model speculation labeled separately.
- Do not share credentials, private server access, or secrets in prompts.

## Good first prompt

“Develop three possible identity systems for Dead Signal DB. Each must support games, software, tools, and experiments without sounding like an agency. Evaluate each for distinctiveness, long-term flexibility, emotional impact, and implementation cost.”

The orchestrator then synthesizes the results and determines whether the brand brief should change.
