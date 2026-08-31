# The Signal Field

## Concept

The Signal Field is the interactive front door to Dead Signal DB. Visitors encounter a living field containing distinct signals, each representing a project or experiment.

The interaction communicates that Dead Signal DB is a changing body of work rather than a static portfolio.

## Core interaction

1. Establish the parent identity and current field state.
2. Show a small number of signals with intentional spatial relationships.
3. Let pointer, touch, and keyboard focus reveal project identity.
4. Let selection resolve into a project preview or dossier.
5. Allow the visitor to enter the project or return to the field.

## Signal states

- Bright or near: active work.
- Stable: live project.
- Flickering: experimental or changing work.
- Dim or distant: paused or archived work.

These states must be backed by real project metadata.

## Experience rules

- The field should be atmospheric but understandable within seconds.
- Animation must never hide project names, links, or status.
- Hover cannot be the only way to discover content.
- The page needs a list/index mode with the same information.
- Effects should be restrained enough that project imagery and copy remain primary.
- Do not add sound by default; if introduced, it must be optional and off until enabled.

## First version

Start with HTML, CSS, and lightweight JavaScript. Use a responsive field of signals, focus/hover states, project previews, and a visible index fallback. Consider canvas or WebGL only when it adds a meaningful interaction that the simpler version cannot provide.
