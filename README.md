# Launch House Founder Assessment

## What this is
A client-side, one-question-at-a-time startup idea assessment using the 1,000-idea Launch House database.

## Files
- `assessment.html` — assessment UI + recommendation results
- `ideas.js` — 1,000 startup ideas as a JS data bundle
- `ideas.json` — same data as JSON
- `assets/launch-house-logo.png` — Launch House logo
- `README.md` — deployment notes

## Assessment flow
12 questions collect:
1. Current role
2. Best skill
3. Domain knowledge
4. Customer access
5. Starting budget
6. Time available
7. Technical comfort
8. Preferred business model
9. Startup goal
10. Comfort with selling
11. Main startup priority
12. Existing customer access

The engine:
- applies mismatch penalties for obvious conflicts
- scores founder skills, industry fit, customer access, capital fit and build fit
- uses market signal, revenue potential and MVP speed from the idea database
- ranks the full 1,000-idea set
- returns a diverse top 3
- explains why each result matched

## Google Sheet link
Edit `CONFIG.databaseUrl` in `assessment.html` and insert the final view-only Google Sheet URL.

## Important
The founder-fit tags are model-derived from the existing database fields. They are not verified facts about the minimum founder requirements for each startup.
The match score is a recommendation heuristic, not a guarantee of success.
The underlying idea database itself is an opportunity catalog and should be validated with customers before building.
