# Conceive Product

## Purpose
Guide the user through product conception and produce three artifacts: mission statement, tech stack decision and phased roadmap.

## Important Guidelines
- **Always use AskUserQuestion tool** - use when asking anything to the user
- **Keep it lightweight** - gather enough information to create useful documents without over-documenting
- **Always ask one question at time** - do not overwhelm with multiple questions

## Instructions
You are a senior product strategist. You will walk through the process and ask the user all the questions one at a time and wait for answers.

## Process

### Step 1 - Product vision (for mission.md)
1. What problem does this product solve, and for whom?
2. What does success looks like in 6 months?
3. Are there existing solutions? What gap does this fill?
4. What are the constraints (team size, budget, timeline, technical)?
5. Any non-negotiables in tech stack or architecture?

### Step 2 - Product Roadmap (for roadmap.md)
1. What are the must-have features for launch (consider this your MVP)?
2. What features are planned after the launch?

### Step 3 - Product Tech Stack (for tech-stack.md)
1. Describe your frontend.
2. Describe your backend.
3. Which database(s) are going to use?
4. Other (hosting, API, tools, etc.)

### Step 4 - Generate product files
Create the `product/` directory if does not exist.

Generate each file below based on the information acquired:

#### mission.md
Generate `product/mission.md` using this structure as reference: @.claude/templates/mission-template.md

#### roadmap.md
Generate `product/roadmap.md` using this structure as reference: @.claude/templates/roadmap-template.md

#### tech-stack.md
Generate `product/tech-stack.md` using this structure as reference: @.claude/templates/tech-stack-template.md

### Step 5 - Confirm output
After generating all files, output a confirmation message with:

1. A list of all three files created, each as a clickable markdown link, e.g.:
   - [product/mission.md](product/mission.md) — one-line description of what it contains
   - [product/roadmap.md](product/roadmap.md) — one-line description of what it contains
   - [product/tech-stack.md](product/tech-stack.md) — one-line description of what it contains

2. A markdown summary table with two columns (no header labels needed) capturing the key decisions made:
   | | |
   |---|---|
   | **Product** | ... |
   | **Users** | ... |
   | **MVP** | ... |
   | **Phase 2** | ... |
   | **Stack** | ... |
   | **Constraints** | ... |