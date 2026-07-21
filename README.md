# GrantPath Europe

GrantPath helps organisations find European funding and prepare a clear plan before applying.

[Watch the product demo](docs/demo.webm)

## Business problem and users

GrantPath helps organisations find European funding and prepare a clear plan before applying. It is useful for companies, universities, public organisations, and teams applying for European grants.

## Key workflows

- Search for funding opportunities.
- Filter opportunities by subject.
- Compare deadlines and requirements.
- Save the best opportunities.
- Create a shared plan for an application.
- Track applications that are being prepared.

## Vue highlights

The product uses Vue to organise separate pages, forms, lists, and smooth screen changes. Shared information stays in one place so every page shows the same result. Automated checks cover the most important actions.

## Java backend highlights

The Java backend uses Spring Boot. It provides real API endpoints to list, search, and create funding task records. It checks incoming information, returns clear errors, exposes a health check, and includes automated Java tests.

## Architecture and state flow

The browser application calls the Java API on port 8080. The Java service checks the request and keeps the shared product information. After a user creates a record, the API returns the saved result and the browser refreshes the list.

## Accessibility and responsive behaviour

Buttons, forms, and links can be used with a keyboard. Labels explain what each field does, and important information is shown with words, not only colours. The layout also adjusts for tablets and phones.

## Run and verify

These commands install the project, check it, and start it on a computer:

```bash
npm ci
npm test
npm run build
npm run dev
npm run backend:test
npm run backend:build
npm run fullstack
```

## Structure

- `backend/` — the Java API, validation, business rules, and tests.
- `scripts/run-full-stack.mjs` — starts the frontend and backend together.
- `src/` — the product pages, actions, and design.
- `docs/demo.webm` — a short video showing the product.
- `package.json` — the commands and packages needed to run it.
- `README.md` — this simple product guide.

## Tradeoffs and roadmap

This project uses sample information and does not connect to a real company system. A future version could connect to official funding sources, add partner invitations, budgets, and approval steps.
