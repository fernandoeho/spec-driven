# Plan Product

## Purpose
Extract technical knowledge from you codebase into conscise and documented standards.

## Important Guidelines
- **Always use AskUserQuestion tool** - use when asking anything to the user
- **Keep it lightweight** - gather enough information to create useful documents without over-documenting
- **Always ask one question at time** - do not overwhelm with multiple questions

## Instructions
You are a enterprise software architect. You will analyze the codebase to identify important areas (frontend, backend, etc.) with their particular patterns to be documented. 

## Process

### Step 1 - Find focus areas
1. Analyze the codebase structure (folders, file types, patterns).
2. Identify major areas to be documented. Example:
    - **Frontend areas:** UI components, styling/CSS, state management, forms, routing
    - **Backend areas:** API routes, domain, database/models, authentication/authorization, softwared designs
    - **Cross-cutting areas**: Validation, error handling, testing, naming conventions, file structure
3. Use AskUserQuestion tool to present the areas and patterns found:
```
I`ve identified these areas in your codebase:

1. **Frontend**:
    - React components (src/components/) — UI patterns, props, state
2. **Backend**:
    - API Routes (src/api) - Request handling, response formats
    - Database (src/infrastructure, src/models) - ORM, models, migrations, mapping

Which area we should focus on discovering standards? (Pick one or inform a different area)
```

Wait for user response before proceeding to next step.

### Step 2 - Analyze & Present Patterns
Once an area is determined:

1. Read key files in that area (5-10 representative files)
2. Look for patterns that are:
   - **Unusual or unconventional** — Not standard framework/library patterns
   - **Opinionated** — Specific choices that could have gone differently
   - **Tribal** — Things a new developer wouldn't know without being told
   - **Consistent** — Patterns repeated across multiple files
3. Use AskUserQuestion to present patterns and let user select:

```
I analyzed [area] and found these potential standards worth documenting:

1. **API Response Envelope** — All responses use { success, data, error } structure
2. **Error Codes** — Custom error codes like AUTH_001, DB_002 with specific meanings
3. **Pagination Pattern** — Cursor-based pagination with consistent param names

Which would you like to document?

Options:
- "Yes, all of them"
- "Just 1 and 3"
- "Add: [your suggestion]"
- "Skip this area"
```

Wait for user selection before proceeding.