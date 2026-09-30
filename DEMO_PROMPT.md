# Prompt for building the Lamma demo with Claude

Attach `README.md` and every image in `screenshots/` to the chat, then paste:

---

I'm a Flutter developer and I built **Lamma (لمّة)**, a group-outings app for Egypt. The attached README describes it, and the attached screenshots are real captures from the running app (Pixel 8, Arabic RTL, plus one in English).

Build me an **interactive product demo** as a single HTML page that I can share with recruiters and link from GitHub.

**What the page should do**
1. **Hero:** the app name in Arabic and English, the one-line pitch ("Group outings for people who don't have a group yet"), and a phone frame showing the home screenshot.
2. **Guided walkthrough:** a phone mockup in the centre that steps through the real user journey using my screenshots, in this order: home → search filters → search results → outing details → booking summary → payment rails → my bookings → booking details → group chat → notifications → padel → wallet. Next/previous buttons, keyboard arrows and swipe. Next to the phone, a short caption for each step saying what the user is doing and **one engineering detail** behind it (take these from the README, e.g. "capacity is enforced in one Postgres function that row-locks the outing").
3. **Arabic ⇄ English toggle** for the captions. Arabic must be real RTL, not mirrored English.
4. **"Under the hood" section:** an architecture diagram (presentation → domain → data → Supabase, with the payment webhook as the only source of payment truth) and the numbers from the README (1,302 tests, 177 migrations, 14 features, 60 merged PRs).
5. **"How I built it" section:** a short timeline: Figma design → UI with mock data → feature-by-feature backend integration (F0–F25) → pair-programming with Claude Code under strict rules. Include the three lessons from the README as short cards.
6. **Footer:** my email (sfhmy7124@gmail.com), and a note that the source is private but available for walkthroughs.

**Style**
- Use the app's own palette: maroon `#580B14` as primary, deep maroon `#36070C` for text and shadows, cream `#FEF3E0` background, gold `#E7B857` accent, green `#2E7D32` for savings badges. Rounded cards, soft shadows, like the screenshots.
- An Arabic-friendly font from Google Fonts (e.g. *Almarai* or *Tajawal*) for Arabic, and a clean sans for English.
- Mobile-friendly: on a phone the walkthrough becomes a vertical swipe.
- Light and dark mode.

**Rules**
- Use only my screenshots for app visuals. Don't invent screens, features or numbers that aren't in the README.
- Keep captions short: one sentence for what the user does, one for how it works.
- Everything in one self-contained file.

When it's done, give me three short variants of the hero headline to choose from.

---

## Optional: a 60–90 second video script

If you also want a screen-recorded video, add this to the same chat:

> Also write a 60–90 second voice-over script for a screen recording of this walkthrough, in Egyptian Arabic, with English subtitles. Structure: the problem (10s) → the journey through the app (45s) → what's under the hood (20s) → call to action (10s). Mark which screenshot is on screen for each line.
