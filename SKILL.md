---
name: cold-email
description: Write, review or rewrite cold emails that get replies, tuned to your business. On first use it asks a few questions about the business, saves the answers as a profile, and then follows them every time, including your red lines. Use when the user asks to cold email, pitch, reach out to, follow up with someone who didn't reply, write subject lines, or improve a cold draft. Also use for "set up cold email", "update my cold email profile" or "add a red line".
---

# Cold email

A cold email has one job: **earn a reply.** It doesn't have to make a sale or book a meeting. It has to get one reply from a busy stranger who reads on a phone and decides in two seconds.

## 0. Load the business profile first

Before writing anything, look for the profile, in this order:

1. `./cold-email-profile.md` (the current project)
2. `~/.claude/cold-email-profile.md` (shared across projects)

**Found:** read it and follow it, including every red line, for the rest of the task. Use only its facts as proof.

**Not found, or the user says "set up cold email":** run the setup below before you write.

**"Update my profile" / "add a red line":** edit the profile in place, show the changed lines, and keep everything else.

### Setup (first run)

Ask these in **one message**, numbered, and say any of them can be skipped:

1. **What do you sell?** One line, plus who it's for.
2. **Who do you email?** For example: buyers, partners, press, investors, dealers. Name the 1–3 main groups.
3. **What proof can you use?** Real numbers, results and customers you're *allowed* to name. Only list what is true and public.
4. **What can you give before asking?** For example: a sample, a free audit, photos, data, a demo video.
5. **Red lines.** What must an email never say or do? For example: no prices, never name competitors, no claims about X, never email existing customers.
6. **How do you sign off?** Your name, role, and a signature or link if you use one.

Then:

- Write the answers into the profile using the template in `profile-template.md`.
- Save it to `~/.claude/cold-email-profile.md`. If the user wants it for one project only, save it to `./cold-email-profile.md`.
- Show the saved profile and say where it lives.
- Never put passwords, API keys or private customer data in the profile.
- Questions that were skipped stay empty in the profile. Don't fill them with guesses.

## 1. Red lines

Red lines are hard stops, not style advice. Check them **before** you write and again before you show the draft.

### Built-in, always on

1. **Never invent anything.** That covers facts, numbers, results, customers, quotes, mutual connections and personal details. If a line needs a fact you don't have, write a visible placeholder: `[PERSONALIZE: their recent launch]`.
2. **Never send.** Write the text and show it. The user sends.
3. **No deception.** No fake "Re:" or "Fwd:" subjects, no pretending you've met, no false urgency or fake deadlines, no posing as someone else.
4. **Don't use private information.** Use only what the person or their company made public for work. Nothing about family, health, religion, politics or their location outside work.
5. **Respect a no.** Never write to someone who opted out or asked to stop. Two follow-ups at most, then stop.
6. **Follow the anti-spam rules where you send.** Use real sender identity and a working way to opt out. If the user's region or industry needs more (an address in the footer, consent first), the email must include it.
7. **No claims you can't back up.** Every number or result must come from the profile or from a source the user gave in this conversation.

### Business red lines

These are the ones listed in the profile. They carry the same weight as the built-in ones.

### When a request crosses a red line

Stop. Name the line in one sentence, then offer the closest version that respects it. For example: "Your profile says no prices in first emails. I can offer to send pricing if they reply." Don't quietly drop the request, and don't bend the line because the user asked twice. Only an edit to the profile changes a red line.

## 2. Gather before writing

You need three things:
- **Who:** name, role and company.
- **What:** what the user wants from them, in one sentence.
- **Why them:** one true, specific reason this email is for this person.

- If tools allow, research the recipient. Look for a recent post, launch, hire, article or event. Pick **one** current detail tied to the reason for writing.
- If you can't find a real hook, use a placeholder. A placeholder gets filled in; a fake compliment gets the email deleted.
- If essentials are missing, ask at most 3 short questions, then stop.

## 3. Writing rules

1. **The first line is about them.** Never open with "I", "we", the company name or "I hope this finds you well". The first line is the preview text.
2. **50–90 words.** Over 125 words fails. It has to read on a phone without scrolling.
3. **One idea, one ask.** Keep the ask small and easy to answer: "Worth a look?", "Want the photos?", "Is this relevant to you?". Never ask for "30 minutes?" up front.
4. **Proof, not adjectives.** One specific fact from the profile beats "innovative" or "leading".
5. **Give before you ask** when the profile lists something to give.
6. **Give an easy out.** "If it's not a fit, no worries." Permission to say no raises replies.
7. **Say "you" more than "I" or "we".**
8. **Sound typed, not crafted.** Use plain words and contractions, with lines of uneven length. Cut em-dashes, lists of three, neat summary lines at the end, and words like "excited", "game-changing", "leverage", "streamline", "touch base" and "just following up".
9. **Plain text.** No images or attachments in a first email. Use links instead, and a normal signature.
10. **Subject line:** 2–6 words in sentence case or lowercase that say what's inside. No hype, no capitals, no "!".

## 4. Shapes

**Press or editor pitch:** what's new, why their readers care, one fact, then offer assets.
> Hi [first name],
> [Hook: their recent story or section, tied to the news.]
> [The news in one line, with the reader's benefit first.]
> [One proof fact.]
> [Offer: photos, data or a sample. One question.]

**Buyer, partner or dealer:** their problem, proof from someone similar, a tiny ask.
> [first name], [hook: something specific they did or said].
> [The problem their customers or team have, in their words.]
> [Proof: a similar customer's result, real only.]
> Worth sending you [the thing you can give]?

**Follow-up:** once, 4–5 business days later, in the same thread. Add something new, like a photo, a result or a mention, and give an easy no. Never "just bumping this". Send a second and last follow-up only if the user wants one, then stop.

## 5. Review checklist

Score every draft out of 10. Fix every fail before you show it.

1. The first line is about the recipient and specific to them. It couldn't go to anyone else.
2. 50–90 words (fails over 125).
3. Exactly one ask: small and phrased as a question.
4. One concrete proof fact, true and taken from the profile.
5. No pitch-speak and no stacked adjectives.
6. "You" outnumbers "I" and "we".
7. The subject line is short and honest, with no hype.
8. Read aloud, it sounds like a person typing between meetings.
9. Nothing invented, and every placeholder is visible.
10. **Every red line is respected, built-in and business. If this one fails, the whole draft fails, whatever the other scores.**

## 6. Output

- By default, write **one** email per recipient: subject, body, word count and score. Offer one other angle only if asked.
- List every placeholder under "Fill in before sending".
- Show the text in chat. Only put it into an email client if the user asks: one draft per recipient, never duplicates. If you redraft, say which earlier drafts to discard.
- Never send.

## Credits

The rules were rewritten in my own words from ideas in these open-source projects:
- [MADEVAL/cold-email-coach](https://github.com/MADEVAL/cold-email-coach): reply as the only goal, the scored checklist, placeholders instead of invented personalization
- [felixleezd/cold-message-writer](https://github.com/felixleezd/cold-message-writer): the first line is about them, sounding typed and not crafted
- [arnabbagxd/cold-email](https://github.com/arnabbagxd/cold-email): give before asking, specific proof, an easy out
- [Cold-IQ/ColdIQ-s-GTM-Skills](https://github.com/Cold-IQ/ColdIQ-s-GTM-Skills): under 100 words, observation-led openers
- [growthenginenowoslawski/coldoutboundskills](https://github.com/growthenginenowoslawski/coldoutboundskills): the structure of a full outbound toolkit
