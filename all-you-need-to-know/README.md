# my-claude-skills
Collection of my personal claude skills

# AllYouNeedToKnow — Claude Interview Intelligence Skill

A Claude skill that turns an interview email into a full, polished Word briefing document — in one step.

Paste the interview email. Get back a downloadable `.docx` with live-researched intel on the company, the interviewer, recent investor news, likely questions, and a sharp game plan. No Googling. No tab-switching. No half-baked LinkedIn stalking at midnight.

---

## What It Does

AllYouNeedToKnow browses the web on your behalf using Claude in Chrome and produces an 8-section Word document covering:

1. **The Company at a Glance** — business model, HQ, team size, exchange listing, key partners
2. **Investor Intelligence** — recent press releases, capital raises, JV deals, drilling results (for mining/exploration companies), financial snapshot with exact figures and dates
3. **Culture** — what it's actually like to work there, sourced from Glassdoor, Reddit, LinkedIn employee posts, and company activity
4. **The Interview Process** — known stages, formats, what trips candidates up
5. **Likely Interview Questions** — 6–8 questions grounded in real research, each with a one-line prep tip
6. **Your Interviewer** — full career history, education, recent LinkedIn posts, communication style, whether they're a CEO/founder or hiring manager, and sharp questions to ask them
7. **Recent News** — key headlines with dates, specific things to reference in the interview, landmines to avoid
8. **Game Plan** — 4–6 sharp, research-grounded recommendations for what to say, what to avoid, and what will make you memorable

---

## What Makes It Different

- **Finds things most candidates miss** — deal terms, drilling results, SEDAR filings, investor narrative, CEO LinkedIn posts from last week
- **Flags when the interviewer is a founder or executive** — changes the entire dynamic and the skill calls it out explicitly
- **Uses live browser research, not training knowledge** — navigates to the company website, LinkedIn, Glassdoor, and news sources in real time
- **Delivers everything in a Word doc** — structured, annotated, ready to read the night before

---

## Requirements

- **Claude** (claude.ai or Claude Code)
- **Claude in Chrome extension** — installed and connected ([download here](https://chromewebstore.google.com/detail/claude/phmlobelhkgpjnkmmfmfehkghibnpami))
- Site permissions granted for: `linkedin.com`, `glassdoor.com`, and the company's own domain
- If Claude in Chrome isn't available, the skill falls back to Claude's native web search tool (enable in Settings → Features → Web Search)

---

## How to Install

### Option A — Install the `.skill` file directly
1. Download `all-you-need-to-know.skill` from this repo
2. In Claude, go to **Settings → Skills**
3. Drag and drop the `.skill` file to install it

### Option B — Copy the SKILL.md manually
1. Open `SKILL.md` from this repo
2. In Claude, go to **Settings → Skills → Create New Skill**
3. Paste the contents of `SKILL.md`

---

## How to Use

**Trigger it by pasting an interview email:**

> "I have an interview coming up — here's the email I received: [paste full email]"

Or trigger it manually:

> "Run AllYouNeedToKnow for [Company Name], I'm interviewing with [Name]"

The skill will:
1. Extract the company name, interviewer, and role from your input
2. Open a browser and research all 5 tracks (company site, investor news, LinkedIn, culture, news)
3. Synthesize everything and generate a Word document
4. Deliver the `.docx` directly in chat

**Tips for best results:**
- Paste the full email thread, not just the company name — the more context, the better
- Make sure Claude in Chrome has permissions for the relevant sites before starting
- Run it again for each new interviewer you meet as you progress through rounds
- Read the full doc the night before; re-read only Section 6 and Section 8 the morning of

---

## Example Output

Built and tested against a real interview at **Mundoro Capital Inc.** (TSXV: MUN). The live research surfaced:
- The CEO (Teo Dechev) was the interviewer — not flagged anywhere in the email
- A US$35M BHP earn-in deal signed 7 months prior with exact royalty terms
- Active drilling that had started 2 weeks before the interview — askable by name
- The CEO's co-founded health-tech/machine vision company — explained her AI interest
- Her LinkedIn posts from the prior week on global copper supply gaps

None of this was in the original email.

---

## Built With

- Claude (Anthropic)
- Claude in Chrome (browser automation via MCP)
- docx-js (Word document generation)
- Skill Creator skill (for building and packaging)

---

## Author

Built by Jahan using Claude's skill system.  
Feel free to fork, improve, and share.

---

## License

MIT — use it, modify it, share it freely.