# cold-email skill

A Claude skill for writing cold emails that get replies, set up around **your** business.

On first use it asks 6 short questions: what you sell, who you email, what proof you can use, what you can give first, your red lines, and how you sign off. It saves the answers as a profile, and every email after that follows them.

## What it does

- **Writes, reviews and rewrites** cold emails, follow-ups and subject lines.
- **Remembers your business** in a plain Markdown profile you can read and edit.
- **Enforces red lines.** There are built-in ones (never invent facts, never send, no fake "Re:", no private details, respect opt-outs, follow anti-spam rules) plus your own. When a request crosses one, it stops, names the line, and offers the closest version that doesn't cross it.
- **Scores every draft out of 10** before showing it. Breaking a red line fails the whole draft.
- **Never sends anything.** You do.

## Install (Claude Code)

```bash
git clone https://github.com/ar-shayeb/cold-email-skill ~/.claude/skills/cold-email
```

Then ask Claude: **"set up cold email"**.

Other agents that read `SKILL.md` files work the same way: put the folder wherever your agent loads skills from.

## Where your profile lives

- `~/.claude/cold-email-profile.md`: shared across all your projects (the default)
- `./cold-email-profile.md`: for one project only, which overrides the shared one

To change it, say "update my cold email profile" or "add a red line: never mention pricing". You can also edit the file directly. The empty template is in [`profile-template.md`](profile-template.md).

The profile stays on your machine. Don't put passwords, API keys or private customer data in it.

## Credits

The rules were rewritten from ideas in these open-source projects. Thank you to their authors:

- [MADEVAL/cold-email-coach](https://github.com/MADEVAL/cold-email-coach)
- [felixleezd/cold-message-writer](https://github.com/felixleezd/cold-message-writer)
- [arnabbagxd/cold-email](https://github.com/arnabbagxd/cold-email)
- [Cold-IQ/ColdIQ-s-GTM-Skills](https://github.com/Cold-IQ/ColdIQ-s-GTM-Skills)
- [growthenginenowoslawski/coldoutboundskills](https://github.com/growthenginenowoslawski/coldoutboundskills)

## License

MIT
