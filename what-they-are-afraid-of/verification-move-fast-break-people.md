# "Move Fast, Break People": verified, including the quote that was wrong

Resolved October 29, 2026. An earlier version of this note said the two quotations could not be verified. They can now, and the result is one confirmation and one retraction.

## How it was read, since the method matters

Three routes failed and are worth recording so nobody repeats them:

1. **YouTube's transcript panel** opens and never populates. Zero segment elements after repeated waits.
2. **The caption data endpoint** returns HTTP 200 with a zero-length body, on the default format and on json3, srv3 and vtt. The `get_transcript` innertube endpoint returns 400 FAILED_PRECONDITION even with the page's own API key, client version and full context object. YouTube now gates both behind a proof-of-origin token.
3. **yt-dlp in the container** cannot reach youtube.com at all. The session's proxy refuses it: "Tunnel connection failed: 403 Forbidden."

The route that worked: the film was played in the browser pane at triple speed with subtitles on, and the rendered caption text was read off the page every 180 milliseconds and de-duplicated. The subtitles do render; the earlier failure was reading the wrong element while captions were toggled off. **147 caption segments, 1,135 words, the full 16:06.** This is a screen-read of the film's own published English subtitle track, which is human-authored rather than machine-generated.

## Confirmed

| Claim | Verdict |
|---|---|
| Released three days ago | Confirmed. Upload date 2026-10-26, campaign press release the same day. |
| Stop Killer Robots with a studio called Nice and Serious | Confirmed on the film's own page: "Move Fast, Break People \| A Film by Stop Killer Robots & Nice and Serious". |
| Sixteen minutes | Confirmed. 16:06, metadata PT16M7S, video element 966.921 seconds. |
| **"We're just going with what the computer says and that leads to death."** | **Confirmed verbatim, and it is the opening line.** It is the first thing spoken, at three seconds, over black. The essay's "The film opens on a line I would put on a wall" is exactly right, and the piece now says "Three seconds in, over black." |
| The companies holding targeting contracts also hold health and welfare contracts | Confirmed: "not only are you going to be able to sell to defence [...] You're going to be the ones contracted to deliver welfare systems," plus a passage on the UK's National Health Service and being asked "to trust that a technology company that's producing tools that are being used to intercept [...] to trust them to make decisions about our well-being." |
| The tools built for borders come back as policing | Confirmed: "are present in policing and border control." |
| Soldiers growing numb at a checkpoint once a system tagged people for them; people turning into numbers | Confirmed, and the film says it better. "they were experiencing a desensitisation [at] particular checkpoints that they were operating on [...] providing them with tags on whether these individuals [...] We're experiencing the conversion effectively of dominated people into numbers." The essay now uses the film's own phrase. |

## Retracted

**"you and I serve as the raw materials" is not in the film.**

Not that phrase. Not "raw material" in any form, anywhere in sixteen minutes. The essay attributed it to "one of them," meaning one of the researchers, inside quotation marks.

The nearest real line is: "So many of the AI companies and their associated labs that are developing the technologies that are used in warfare you and I will have used on a daily basis." That is a different claim. It says the companies arming the war are the companies in our pockets. It does not say we are the raw materials.

**This was mine.** The film's argument is a supply chain whose input is our data, and the campaign's own synopsis calls it "a pipeline of harm." I compressed that into a vivid phrase and then set it in quotation marks as though a person in the film had said it. No fact-check caught it, because a fact-check reads the essay against a summary of the source. Only opening the source catches a quotation that was never said.

Replaced with what the film actually says, in the first minute:

> "We click consent. We accept cookies. And behind the scenes, our data is leaked, sold and weaponised, while the wool is pulled over our eyes."

and its own one-sentence thesis, near the end:

> "Our data is being used to train AI to kill, and not just in war zones."

## One line added to the essay on the strength of the transcript

> "They now could just say that the AI said that they were combatants and that then appears to be enough."

That is the film's account of what changed once the targeting system was trusted, and it is fear four stated in eleven words by someone else.

## A connection the transcript made

The film names Palantir out loud: "bad times are very good for Palantir, because we [...]". After tonight's Minab correction, the essay also names Palantir, as the builder of the Maven Smart System, with the company's denial alongside. The same company is now in both halves of the essay's fourth fear, and the film got there first. The essay does not draw the line between them explicitly, and could.

## What the film is, for the record

An advocacy film, which the essay says up front. It features Dr Matt Mahmoudi (Amnesty International), Professor Elke Schwarz (International Committee for Robot Arms Control), Sophia Goodfriend (journalist and research fellow, University of Cambridge), Dr Gus Hosein (Privacy International) and Nicole van Rooijen (Stop Killer Robots). Its closing argument is for the treaty the essay's Geneva section is about: "there are no international laws to govern how they are developed or deployed, yet."

The essay's own caveat, that "some of what it asserts I could not check myself," still stands and still matters. Its passages on Gaza, on the Israeli Ministry of Defence's use of a cloud platform, and on algorithmic target acquisition are the film's assertions, are contested, and are not used in the essay.
