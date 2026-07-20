# GrantPath Europe

GrantPath is a European funding-intelligence and bid-delivery workspace. It connects opportunity discovery, eligibility qualification, portfolio shortlisting and consortium submission planning.

[Watch the verified product demo](docs/demo.webm)

## Business problem and users

Public bodies, consultancies, universities and SMEs lose time across disconnected call portals and spreadsheets. Funding teams use GrantPath to focus capacity on high-fit programmes and create governed bid workspaces.

## Key workflows

- Search and filter current funding calls by domain.
- Compare programme, deadline, eligibility and organisational fit.
- Build a qualified shortlist.
- Review portfolio readiness and evidence gaps.
- Create a validated consortium bid workspace.
- Track active submissions and review states.

## Vue technical highlights

Vue 3 Composition API, typed setup scripts, Pinia domain state, Vue Router product areas, computed selectors, TransitionGroup feedback, reusable cards, validated controlled forms and Vitest store tests.

## Architecture and state flow

The Pinia store centralises calls, shortlists and bids. Route views own transient search/form state and consume computed collections. Reusable cards communicate narrow user intent through typed store actions.

## Accessibility and responsive behaviour

Search, filters and forms are explicitly labelled, feedback uses status regions, actions have descriptive names and grids reflow across desktop and mobile viewports.

## Run and verify

```bash
npm ci
npm test
npm run build
npm run dev
```

## Structure

- `src/views` — funding radar, shortlist and bid routes
- `src/components/MediaCard.vue` — reusable opportunity card
- `src/store.ts` — Pinia portfolio state
- `src/router.ts` — route map

## Tradeoffs and roadmap

Calls and scores are illustrative. A production roadmap includes official portal feeds, eligibility rules, organisation profiles, partner discovery, evidence reuse, work-package budgeting, approval gates and submission exports.
