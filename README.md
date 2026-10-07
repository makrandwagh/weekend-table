# Weekend Table

A lightweight web app that answers "where should we eat this weekend?" from a personal list of restaurants, with a one-click handoff to an AI assistant for a second opinion.

**[Try it live](https://makrandwagh.github.io/weekend-table/)**

## The problem

Weekend dinner decisions stall because the options live in my head, filtered by who's coming, budget, and mood. [Add one sentence in your own words.]

## How it works

1. Filter by cuisine, price, and kid-friendliness.
2. Get three random matches from the filtered list.
3. Click "Copy prompt for Claude" to generate a prompt containing the filtered list, then paste it into Claude for ranked picks and similar places to try.

## Product decisions

- **Data separate from code:** restaurants live in `restaurants.json`, so updating the list requires no code changes.
- **No API key, no backend:** the AI step is a copy-paste handoff. This keeps the app free to run and removes key-management risk. The tradeoff is one manual step.
- **Static hosting:** GitHub Pages, so there is nothing to maintain.

## v2 ideas

- Call the Claude API directly so recommendations appear in-page
- Add weather and distance as filters
- Let each family member vote
- Track where we've been to avoid repeats

## Built with

HTML, CSS, vanilla JavaScript.
