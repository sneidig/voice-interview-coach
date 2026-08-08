# Voice Interview Coach

Nine markdown files that turn a Claude conversation into an interview coach you talk to out loud.

Adapted from the [Interview Coach skill](https://github.com/noamseg/interview-coach-skill) by [Noam Segal](https://www.linkedin.com/in/noamsegal/), MIT licensed. The workflows, the five scoring dimensions, the drill progression, and the debrief sequence are his. This is a much smaller thing carved out of it, built for one feature it doesn't have.

## What this adds

Claude's voice mode can't load skills, since skills need the code execution environment and voice mode doesn't have one. These files carry their instructions inline instead. Attach one to a chat, switch to voice, and practice by talking.

## Quick Start

1. Clone the repo:

```bash
git clone https://github.com/sneidig/voice-interview-coach.git
cd voice-interview-coach
```

Or [download it as a ZIP](https://github.com/sneidig/voice-interview-coach/archive/refs/heads/main.zip) and unzip.

2. Make your profile:

```bash
cp my-profile-template.md my-profile.md
```

Open `my-profile.md` and fill in the Basics section at the top. Five fields. Leave the rest blank, sessions fill those in.

3. Start a new chat in the Claude app and attach `modules/01-story-builder.md`. Send it.

4. Attach `my-profile.md` in a second message. One file per message, or voice sessions struggle to read them.

5. Switch to voice mode and say "let's start."

6. When you're done, switch back to text and ask for your updated profile. Save what it gives you over `my-profile.md`.

Requires any Claude plan, free included. Works on desktop, tablet, or phone.

**On a tablet?** Start the chat on a computer where attaching files is easier, then open that same conversation on the tablet and switch to voice there. Chats sync across devices.

**One module per conversation.** They give feedback at different moments, so mixing them gets muddled.

## The modules

Numbered in the order you'd use them across a job search. Start with `01-story-builder.md`, since the drills and mocks need stories to work with.

| File | What it does | How long |
|---|---|---|
| `01-story-builder.md` | Surfaces your stories out loud and sharpens them | 20 to 40 min |
| `02-pitch.md` | Tell me about yourself, plus the 10, 30, and 60 second versions | 20 to 30 min |
| `03-practice-drills.md` | Short drills with feedback every round. Compression, pushback, pivots, gap handling | 15 to 30 min |
| `04-mock-interview.md` | Full simulated interview, 4 to 6 questions, no feedback until the end | 30 to 45 min |
| `05-role-pressure-test.md` | A specialist in your field attacks your best project | 15 to 25 min |
| `06-recruiter-screen.md` | Role-plays the salary expectations question until it stops rattling you | 15 to 25 min |
| `07-pre-interview-hype.md` | Warmup 20 minutes before the real thing | Under 10 min |
| `08-debrief.md` | Same-day capture after a real interview | 10 to 20 min |
| `09-negotiation.md` | Rehearses the offer call | 20 to 30 min |

## The profile file

Claude doesn't remember anything between conversations, so each session starts cold without it. `my-profile.md` is what carries your stories, scores, and interview history forward.

Update it at the end of every session (step 6 above) and it builds up over time. It's in `.gitignore`, so your personal details never get committed.

## What these cover

The parts of interview prep that work as a conversation.

Answers are scored on the same five dimensions as the original: Substance, Structure, Relevance, Credibility, and Differentiation. You get the drill ladder, mock formats including panel, earned-secret extraction, story red-teaming, signal reading in the debrief, and the anchoring logic behind the salary conversation.

Not in here: transcript analysis, resume and LinkedIn work, JD decoding, outreach coaching, company research and prep briefs, role-fit assessment, and the calibration engine that checks whether practice scores predict real outcomes.

Those come down to two things an attached file can't do. Some need computed state across sessions. The rest is document work, where reading a resume out loud is worse than editing it on a screen. The [full skill](https://github.com/noamseg/interview-coach-skill) does all of it, and it's where to go once you're back at a desk.

## Using both together

The full skill already supports spoken practice. Pair it with a dictation tool like Superwhisper and you can talk through mock interviews while keeping the scoring, the transcript analysis, and the coaching state that carries between sessions. That's the stronger setup when you're at your desk.

These modules are for the times you're not. A tablet on the couch, a phone before a call, a machine without your tools installed. Voice mode handles the speaking on its own, so there's nothing to install.

They also chain. Talk through a mock here, then bring the transcript to the full skill and run `analyze` for scoring that sticks around.

## License

MIT, same as the original. See `LICENSE`.
