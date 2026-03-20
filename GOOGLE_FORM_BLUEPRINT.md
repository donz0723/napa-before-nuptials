# Google Form Blueprint — Napa Before Nuptials

**Form title:** Napa Before Nuptials · Guest Details
**Form description:** Fill this out so we can plan every detail of the weekend around you — from hotel rooms to Napa wine preferences to Saturday activities. Takes about 3 minutes!

---

## How to build this form

1. Go to [forms.google.com](https://forms.google.com) — use a **personal @gmail.com account** (not a work/school account, which may block the embed)
2. Create a new blank form
3. Set the title and description above
4. Add each question below in order
5. When done: click **Send → `<>` (Embed icon)** → copy the `src` URL
6. Paste into `index.html` as instructed at the bottom of this file

---

## Questions

---

### Q1 — Full name
- **Type:** Short answer
- **Required:** Yes
- **Helper text:** *(none needed)*

---

### Q2 — Email address
- **Type:** Short answer (set validation to Email)
- **Required:** Yes
- **Helper text:** We'll use this for updates and coordination only.

---

### Q3 — Phone number
- **Type:** Short answer
- **Required:** No (mark Optional)
- **Helper text:** For the group chat we'll set up closer to the trip. Totally optional!

---

### Q4 — Dietary restrictions & allergies
- **Type:** Checkboxes
- **Required:** Yes
- **Options:**
  - Vegetarian
  - Vegan
  - Gluten-free
  - Dairy-free
  - Nut allergy (severe / EpiPen)
  - Shellfish allergy
  - Kosher or Halal
  - None — I eat everything!
- **Helper text:** Check all that apply. We'll share this with restaurants and the winery for the Napa lunch.

---

### Q5 — Anything else about your diet?
- **Type:** Paragraph (long text)
- **Required:** No (mark Optional)
- **Helper text:** Please note if something is a **medical allergy** vs. a preference — it helps us flag it to caterers appropriately.

---

### Q6 — Hotel room preference
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - King bed — one large bed (great for solo or sharing with a close friend)
  - Double Queen — two queen beds (great for sharing with someone you don't know as well)
  - No preference — assign me wherever!
- **Helper text:** We're staying at The Westin St. Francis, Union Square.

---

### Q7 — Are you comfortable being matched with a roommate you may not know well?
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - Yes, no problem — match me with whoever needs a roommate
  - I'd prefer to room with someone I already know (name them in the next question)
  - I'm interested in having my own room — I'll be in touch about solo pricing
- **Helper text:** This helps us pair people thoughtfully. No wrong answer!

---

### Q8 — Roommate preference
- **Type:** Short answer
- **Required:** No (mark Optional)
- **Helper text:** If you have a specific person in mind, write their full name as it appears on their RSVP. Leave blank if you have no preference or chose "no problem" above.

---

### Q9 — When do you plan to arrive on Thursday, August 6?
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - Before noon (Thursday morning)
  - 12pm – 3pm (early afternoon)
  - 3pm – 6pm (late afternoon)
  - 6pm – 9pm (evening)
  - After 9pm (late night)
  - Not arriving Thursday — I'll join the group Friday
  - I haven't booked flights yet
- **Helper text:** We're planning a group dinner Thursday evening — this helps us time the reservation.

---

### Q10 — Wine preferences for our Napa day (Friday)
- **Type:** Checkboxes (can select multiple)
- **Required:** Yes
- **Options:**
  - Reds
  - Whites
  - Rosé
  - Sparkling / Champagne
  - All of the above — I love it all!
  - Non-drinker — but very excited to be in Napa!
- **Helper text:** We'll use this to choose wineries with the right tasting menus for the group.

---

### Q11 — Saturday morning: Yoga class
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - Yes — count me in!
  - Maybe — I'll decide closer to the day
  - No thanks
- **Helper text:** We're looking at a private yoga class Saturday morning. We need a headcount to book, so even a "maybe" helps!

---

### Q12 — Saturday: Spa treatments
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - Yes, definitely — book me in!
  - Maybe — tell me more about options and pricing
  - No thanks
- **Helper text:** The Westin has an on-site spa (Iridium Spa). This is separate from yoga — you can do both, either, or neither!

---

### Q13 — Sunday: Outside Lands Festival (optional add-on)
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - Yes, I'm staying Sunday and want to go to Outside Lands
  - Yes, I'm staying Sunday but planning my own day
  - No — I'll be flying home Sunday
  - Not sure yet
- **Helper text:** One-day Sunday tickets are self-purchased (~$150). Please reach out before buying so we can coordinate! Most guests are flying home Sunday — totally fine either way.

---

### Q14 — T-shirt / swag size
- **Type:** Multiple choice (pick one)
- **Required:** Yes
- **Options:**
  - XS
  - S
  - M
  - L
  - XL
  - XXL
- **Helper text:** We'll be ordering unisex sizing — size up if you prefer a looser fit.

---

### Q15 — Anything to celebrate this weekend?
- **Type:** Short answer
- **Required:** No (mark Optional)
- **Helper text:** Birthday? Anniversary? Promotion? New job? We want to celebrate YOU too — spill it!

---

### Q16 — A message to the bride 💌
- **Type:** Paragraph (long text)
- **Required:** No (mark Optional)
- **Helper text:** Donna will read every single one.

---

### Q17 — Anything else we should know?
- **Type:** Paragraph (long text)
- **Required:** No (mark Optional)
- **Helper text:** Special considerations, questions, requests — anything not covered above.

---

## After building the form

### Get your embed URL
1. Click **Send** (top right)
2. Click the **`<>`** tab (Embed)
3. Copy the URL inside `src="..."` — it ends with `?embedded=true`

### Paste into index.html
Find this section around **line 1131** and replace both placeholders:

```html
<!-- iframe src — paste URL WITH ?embedded=true -->
<iframe
  src="PASTE_YOUR_EMBED_URL_HERE?embedded=true"
  title="Napa Before Nuptials — Guest Details">
  Loading…
</iframe>

<!-- fallback link — paste URL WITHOUT ?embedded=true -->
<div class="form-fallback">
  Can't see the form?
  <a href="PASTE_YOUR_FORM_URL_HERE" target="_blank" rel="noopener noreferrer">
    Open it in a new tab ↗
  </a>
</div>
```

### Final step — set iframe height
After pasting the URL and viewing the live form:
1. Open the form link in a browser
2. Open DevTools (F12) → measure the full height of the form
3. In `index.html`, find `.form-shell iframe` in the CSS (~line 822) and confirm the height is set correctly (already updated to 1200px desktop / 1600px mobile)

---

## Recommended Google Form settings

- **Collect email addresses:** Off (we have our own email question — avoids duplicates)
- **Limit to 1 response:** On (requires sign-in, prevents accidental duplicates — recommended)
- **Confirmation message:** Customize to something warm, e.g. *"Thank you! We can't wait to celebrate with you and Donna in August. 🥂"*
- **Progress bar:** On (helps guests see they're almost done)

---

*Blueprint generated: 2026-03-19 · Napa Before Nuptials · August 6–9, 2026*
