# Voice Interview Coach

Nine markdown files you attach to a chat to run interview coaching by voice.

Adapted from the [Interview Coach skill](https://github.com/noamseg/interview-coach-skill) by [Noam Segal](https://www.linkedin.com/in/noamsegal/), MIT licensed. The workflows, the five scoring dimensions, the drill progression, and the debrief sequence are his. This is a much smaller thing carved out of it, built for one feature it doesn't have.

## What this adds

Voice mode doesn't load skills, since skills run in the code execution environment and voice mode doesn't have one. These files carry their workflow inline instead, so you can attach one, switch to voice, and run a session hands-free.

## Quick Start

1. Get the files.

```bash
git clone https://github.com/YOUR-USERNAME/voice-interview-coach.git
cd voice-interview-coach
```

Or download a single module straight from `modules/` if you only want one.

2. Make your profile.

Copy `my-profile-template.md` and name the copy `my-profile.md`. Fill in the Basics section, which is five fields and takes a couple of minutes. Leave everything below it empty, since sessions fill those in for you.

Skip this step if you just want to try a module. It works without a profile.

3. Start the chat on a desktop and attach the files.

Open a new chat in the Claude app. Attach `modules/01-story-builder.md` and send that message. Then attach `my-profile.md` in a second message.

One file per message. Sending both together makes voice sessions struggle to read them.

Desktop is just easier for picking files. The chat syncs across your devices, so where you start it doesn't lock you in.

4. Switch to voice, on whatever device you want.

Open that same conversation on your tablet or phone, switch to voice mode, and say "let's start." Now put the screen down and talk.

If you'd rather stay on the desktop, that works too. The point is that the files are already in the conversation, so voice mode has everything it needs.

5. Save what you did.

When the session ends, go back to that conversation on your desktop, switch out of voice back to text, and ask for your updated profile. You'll get the whole `my-profile.md` back with the session's results already merged in. Save it over your copy.

That's how scores, stories, and interview history build up across sessions.

Requires any Claude plan. The free tier is enough.

**One module per session.** They give feedback at different points, so running several at once gets muddled. A new chat costs nothing.

Nothing in these files is Claude-specific. They're plain markdown with no special syntax, so they should port to any assistant that takes an attachment and does voice, though I've only run them in Claude.

## The modules

They're numbered in the order you'd use them across a job search. Start at the top and work down, or jump to whichever one matches where you are.

| File | What it does | How long |
|---|---|---|
| `01-story-builder.md` | Surfaces stories out loud and sharpens them | 20 to 40 min |
| `02-pitch.md` | Tell me about yourself, plus the 10, 30, and 60 second versions | 20 to 30 min |
| `03-practice-drills.md` | Short drills with feedback every round. Compression, pushback, pivots, gap handling | 15 to 30 min |
| `04-mock-interview.md` | Full simulated interview, 4 to 6 questions, no feedback until the end | 30 to 45 min |
| `05-role-pressure-test.md` | A specialist in your field attacks your best project | 15 to 25 min |
| `06-recruiter-screen.md` | Role-plays the salary expectations question until it stops rattling you | 15 to 25 min |
| `07-pre-interview-hype.md` | Warmup 20 minutes before the real thing | Under 10 min |
| `08-debrief.md` | Same-day capture after a real interview | 10 to 20 min |
| `09-negotiation.md` | Rehearses the offer call | 20 to 30 min |

Start with `01-story-builder.md`. The drills and mocks need material to work with, and that's where the material comes from.

## What these cover

The parts of interview prep that work as a conversation.

Answers are scored on the same five dimensions as the original: Substance, Structure, Relevance, Credibility, and Differentiation. You get the drill ladder, mock formats including panel, earned-secret extraction, story red-teaming, signal reading in the debrief, and the anchoring logic behind the salary conversation.

Not in here: transcript analysis, resume and LinkedIn work, JD decoding, outreach coaching, company research and prep briefs, role-fit assessment, and the calibration engine that checks whether practice scores predict real outcomes.

Those come down to two things a single attached file can't do. Some of them need computed state across sessions. The rest is document work, where reading a resume out loud is worse than editing it on a screen. The [full skill](https://github.com/noamseg/interview-coach-skill) does all of it, and it's where to go once you're back at a desk.

## Using both together

The full skill already supports spoken practice. Pair it with a dictation tool like Superwhisper and you can talk through mock interviews while keeping the scoring, the transcript analysis, and the coaching state that carries between sessions. That's the stronger setup when you're at your desk.

These modules are for the times you're not. A tablet on the couch, a phone before a call, a machine without your tools installed. Voice mode handles the speaking on its own, so there's nothing to set up.

They also chain. Talk through a mock here, then bring the transcript to the full skill and run `analyze` for scoring that sticks around.

## License

MIT, same as the original. See `LICENSE`.
