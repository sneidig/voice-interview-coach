# Voice Interview Coach

Nine markdown files you attach to a chat to run interview coaching by voice.

Adapted from the [Interview Coach skill](https://github.com/noamseg/interview-coach-skill) by [Noam Segal](https://www.linkedin.com/in/noamsegal/), MIT licensed. The workflows, the five scoring dimensions, the drill progression, and the debrief sequence are his. This is a much smaller thing carved out of it, built for one feature it doesn't have.

## What this adds

Voice mode doesn't load skills, since skills run in the code execution environment and voice mode doesn't have one. These files carry their workflow inline instead, so you can attach one, switch to voice, and run a session hands-free.

## How to use it

1. Download the module you want from `modules/`.
2. Start a new chat in the Claude app.
3. Attach the module file and send it.
4. If you're using `my-profile.md`, attach it in a second message.
5. Switch to voice mode.
6. Say "let's start."

Attach one file per message. Sending the module and your profile together in the same message makes voice sessions struggle to read them.

One module per session too. They give feedback at different points, so running several at once gets muddled. A new chat costs nothing.

Works on iPad, Android tablet, phone, or desktop. Free plan included.

Nothing in these files is Claude-specific. They're plain markdown with no special syntax, so they should port to any assistant that takes an attachment and does voice, though I've only run them in Claude.

## The modules

| File | What it does | How long |
|---|---|---|
| `01-mock-interview.md` | Full simulated interview, 4 to 6 questions, no feedback until the end | 30 to 45 min |
| `02-practice-drills.md` | Short drills with feedback every round. Compression, pushback, pivots, gap handling | 15 to 30 min |
| `03-story-builder.md` | Surfaces stories out loud and sharpens them | 20 to 40 min |
| `04-debrief.md` | Same-day capture after a real interview | 10 to 20 min |
| `05-pre-interview-hype.md` | Warmup 20 minutes before the real thing | Under 10 min |
| `06-pitch.md` | Tell me about yourself, plus the 10, 30, and 60 second versions | 20 to 30 min |
| `07-recruiter-screen.md` | Role-plays the salary expectations question until it stops rattling you | 15 to 25 min |
| `08-negotiation.md` | Rehearses the offer call | 20 to 30 min |
| `09-role-pressure-test.md` | A specialist in your field attacks your best project | 15 to 25 min |

Start with `03-story-builder.md` if you're starting from scratch. You need material before drills are worth much.

## The profile file

Chats don't carry over, so a module starts fresh each time.

Copy `my-profile-template.md` to `my-profile.md` and fill in your target role and background. Attach it in a second message after the module, then start. Most modules end by offering a block you can paste back in, so it builds up as you go.

It's gitignored. Your copy stays on your machine.

## License

MIT, same as the original. See `LICENSE`.
