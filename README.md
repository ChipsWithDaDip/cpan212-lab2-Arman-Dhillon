# Tool Library API

<!-- I enjoyed how this lab had step by step instructions and the code had sections outlining which part needed to be added which made it easier for me to follow along and understand-->

Live: <!-- your Render address, for example https://cpan212-lab2-jane-doe.onrender.com/api/tools -->

## Run it

```bash
npm install
cp .env.example .env
npm run dev
```

The API runs at http://localhost:4000. Set `PORT` in `.env` to use a different port.

## Routes

| Method | Path | What it does |
|---|---|---|
| GET | `/api/tools` | Every tool. `?category=garden` keeps only one category |
| GET | `/api/tools/:id` | One tool, or 404 |
| POST | `/api/tools` | Create a tool (201), or 400 with the invalid fields |
| PUT | `/api/tools/:id` | Replace a tool's fields (200), 400 or 404 |
| DELETE | `/api/tools/:id` | Remove a tool (204), or 404 |

## Testing

```bash
npm run check
```

This tries every route and prints which checks pass.

## AI use

<!--I used ChatGPT to identify a few errors in my code which ended up being typing mistakes, and to better understand step 6-->
