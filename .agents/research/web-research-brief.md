# Web research brief — Atrest: Quit Vaping

*Paste everything below the line into a fresh chat that has web search and page reading switched on. Run each part as its own chat if the answers get long. Paste the results back to the lead in Claude Code.*

---

You are doing research for a small iOS app, "Atrest: Quit Vaping", made by one developer in Belgium and sold on EU App Stores in English, French and Dutch. Don't research Atrest itself, except in Part C. Don't give marketing advice or opinions. Report only what you find, in the formats below.

**Rules for all parts**
- Quote only text you saw on a page you actually opened. Copy it exactly. Never paraphrase, translate or combine text inside quote marks.
- Give the URL for every fact and every quote.
- If you can't find something, write NOT FOUND. Never guess or fill gaps.
- Search-result snippets don't count as sources. Open the page.
- Don't include usernames, real names, ages, locations or other personal details. The URL is the only attribution.
- If a site won't load, list it under "Failed sources" and move on.

## Part A — Competing apps (Belgian, French and Dutch App Stores)

Find up to 10 iOS apps that are mainly about quitting vaping or nicotine and are available in Belgium, France or the Netherlands. Search terms to try: "quit vaping", "arrêter de vapoter", "stoppen met vapen", "stop vapen", "quit nicotine", "arrêter la cigarette électronique". Useful sources: apps.apple.com pages for the be, fr and nl stores, and the iTunes Search API (`https://itunes.apple.com/search?term=quit+vaping&country=be&entity=software`).

Leads to check (unverified): Puff Count, Kwit ("Stop voorgoed met roken"), Habit Break, Quit Vaping (Jonathan Kopp), Puffless, Smoke Free.

For each app, report:
- Name | Developer | App Store URL (and which country store)
- Subtitle (exact)
- Price model, with prices and currency as shown
- Rating and number of ratings (which country)
- Top 5 features, from the listing
- Account or sign-up required? (yes / no / unclear, and where you saw it)
- Health or outcome claims, quoted exactly (e.g. success rates, "quit in X days"), or NONE SEEN
- Languages offered
- Does it use streaks, badges, scores or leaderboards? (yes / no / unclear, with a quote)
- Does it have an AI chat or coach? (yes / no, with a quote)

Then: "Failed sources" and "Gaps" (max 3 bullets).

## Part B — How real people talk about quitting vaping

Collect 30–40 exact quotes, about 60% English and the rest French or Dutch. Good sources: Reddit (r/QuitVaping, r/stopvaping, r/QuitNicotine, and quitting threads in r/belgium, r/france, r/thenetherlands), public App Store reviews of the apps from Part A (be, fr and nl stores), and French or Dutch forums such as Doctissimo or Que Choisir.

Tag each quote with one theme:
- MOMENT: what a craving moment is like, what they do with their hands or time
- SLIP: slipping, relapsing, shame, starting over
- APPS: what they like or hate in quit apps (streaks, counters, games, ads, paywalls, accounts, AI coaches)
- PRIVACY: wanting it private or anonymous
- WHY: why they want to quit
- OTHER

One line per quote:
`[THEME] [LANG] "exact quote, max 40 words, cuts marked with …" — URL`

Then: "Failed sources" and a count per theme.

## Part C — Check one page

Open https://atrest.app/privacy.html and report, quoting exactly:
1. Does it load?
2. Who runs the app, and in which country?
3. Does it name Anthropic and/or Amazon Web Services?
4. Where is AI chat data processed? Is it kept, and for how long?
5. What does it say about voice notes and speech-to-text?
6. What does it say about analytics, crash reporting, tracking or third-party code?
7. Minimum age?
8. Last-updated date?
9. Anything that conflicts with: "Everything stays on your phone. No account, no analytics, no third-party code. Chat goes through our server to an AI, both in the EU, and neither keeps it. Voice notes are transcribed on the phone and never sent anywhere."
