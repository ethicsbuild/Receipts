# Receipts

The conversations behind my AI-written pieces, published as they happened.

Claude writes the words. I bring the seed and the seeing, and I do the refusing. I say that at the bottom of everything I publish. But anyone can put "made with AI" on a page. This repo is where you can check whether I earned mine.

## What's here

One record per piece. Each has:

- the full conversation that produced it, unedited
- every draft, including the ones I rejected
- a breakdown of which lines are mine, which are my ideas in Claude's words, and which are Claude's alone
- notes wherever the machine got something wrong

My spoken lines are transcribed as I said them, with the false starts and the swearing left in. Where I changed anything, like protecting details about my kids, the record says so and shows where.

## Records

| Piece | Published | Record |
|---|---|---|
| [The Scarlet Letter](https://gagecasswoodle.substack.com/p/the-scarlet-letter) | September 26, 2026 | [scarlet-letter-process-record.md](scarlet-letter-process-record.md) |
| [Confidently Wrong About a Toilet](https://gagecasswoodle.substack.com/p/confidently-wrong-about-a-toilet) | October 10, 2026 | [confidently-wrong/confidently-wrong-process-record.md](confidently-wrong/confidently-wrong-process-record.md) (redacted; see the note at the top of the record) |
| [A Drone With Hands](https://gagecasswoodle.substack.com/p/a-drone-with-hands) | October 14, 2026 | [a-drone-with-hands/a-drone-with-hands-process-record.md](a-drone-with-hands/a-drone-with-hands-process-record.md) (redacted; the phone call it draws on is not published) |
| [What a Dead Kid Buys You](https://gagecasswoodle.substack.com/p/what-a-dead-kid-buys-you) | October 21, 2026 | [what-a-dead-kid-buys-you/what-a-dead-kid-buys-you-process-record.md](what-a-dead-kid-buys-you/what-a-dead-kid-buys-you-process-record.md) (one passage about a later piece held back) |
| [What They Are Afraid Of](https://gagecasswoodle.substack.com/p/what-they-are-afraid-of) | October 29, 2026 | [what-they-are-afraid-of/what-they-are-afraid-of-process-record.md](what-they-are-afraid-of/what-they-are-afraid-of-process-record.md) (one day of the conversation is lost and the record says where) |

## Reading the records

Each record also has a page where the two voices look different: a person's words in a book typeface, the machine's in a code typeface. My mother asked for that, so you never have to guess who is talking.

- [The Scarlet Letter](https://ethicsbuild.github.io/Receipts/published/scarlet-letter-process-record.html)
- [Confidently Wrong About a Toilet](https://ethicsbuild.github.io/Receipts/published/confidently-wrong-process-record.html)
- [A Drone With Hands](https://ethicsbuild.github.io/Receipts/published/a-drone-with-hands-process-record.html)
- [What a Dead Kid Buys You](https://ethicsbuild.github.io/Receipts/published/what-a-dead-kid-buys-you-process-record.html)
- [What They Are Afraid Of](https://ethicsbuild.github.io/Receipts/published/what-they-are-afraid-of-process-record.html)

The .md files are the records of reference. The styled pages are the same text, formatted.

## Other records

Receipts that aren't about a piece of writing, but about the work itself, including where it went wrong.

| Record | Date | File |
|---|---|---|
| The E.D.A.I. shield says "watching." Almost. | October 8, 2026 | [edai-shield/edai-shield-record.md](edai-shield/edai-shield-record.md) |
| Field Test 001: status and outreach to TypeSafe | October 13, 2026 | [field-test-001/status-2026-10-13.md](field-test-001/status-2026-10-13.md), [field-test-001/typesafe-outreach.md](field-test-001/typesafe-outreach.md) |

## Anchored on Hedera

Each record is fingerprinted on the Hedera public ledger, so anyone can check that it has not been changed since. This proves the files are unchanged. It does not prove they are complete or true.

Topic [0.0.10897644](https://hashscan.io/mainnet/topic/0.0.10897644), "Proof of Life: Authorship Records (Gage Cass Woodle)". Only Gage's key can post to it.

| Piece | Message | Timestamp (UTC) | Version anchored |
|---|---|---|---|
| The Scarlet Letter | [#1](https://hashscan.io/mainnet/topic/0.0.10897644) | 2026-09-30 18:35:17 | commit b3158be |
| A Drone With Hands | [#3](https://hashscan.io/mainnet/topic/0.0.10897644) | 2026-10-14 22:00:24 | commit 27c232b |
| What They Are Afraid Of | [#7](https://hashscan.io/mainnet/topic/0.0.10897644) | 2026-10-29 17:04:08 | commit 8bfa2da |
| Confidently Wrong About a Toilet | [#8](https://hashscan.io/mainnet/topic/0.0.10897644) | 2026-10-29 17:12:46 | commit bec5ffd |
| What a Dead Kid Buys You | [#9](https://hashscan.io/mainnet/topic/0.0.10897644) | 2026-10-29 17:13:29 | commit e8ad4ed |

Messages #2, #4, #5 and #6 are duplicates, each one byte for byte identical to the record before it: #2 duplicates #1, and #4, #5 and #6 duplicate #3. They were posted when a script was re-run before the first post had shown up on the network. They change nothing, and #1, #3, #7, #8 and #9 are the anchors. The three duplicates of #3 were found on October 29, 2026, while the next record was being anchored. Until then this README and the A Drone With Hands process record both said one message went up that day. That was wrong, and this paragraph is the correction.

To check: download the record and the published snapshot at commit b3158be and compare their SHA-256 hashes with the ones in the message.

- scarlet-letter-process-record.md: aa0d134f9a99c15f4f5f094ffcd668a989f831d3adbf39109069704a9b7c8b4a
- published/the-scarlet-letter.html: 1afb854d33731eefb6460ead830fcbaa118a1868595be762f87cd3ef49d59a91

For A Drone With Hands, at commit 27c232b:

- a-drone-with-hands/a-drone-with-hands-process-record.md: 44e5ae0623c16a73889d8c6e94f8581859377ab59cb987063cac62b7b8d644ce
- published/a-drone-with-hands-process-record.html: 032b5c7858cee88c93527e7830aca41d041f3ea56ea526a04dbe2ade63ab09d3

For What They Are Afraid Of, at commit 8bfa2da:

- what-they-are-afraid-of/what-they-are-afraid-of-process-record.md: a821b97de5491ceb755c495c2bc78870a681ad3d1dcd10fec716af58781cafa7
- published/what-they-are-afraid-of-process-record.html: a4f8675b7eec6fce71c21d70a666881dc6ae6c1f9c82ac865e7d2572e5d8f2b1

For Confidently Wrong About a Toilet, at commit bec5ffd:

- confidently-wrong/confidently-wrong-process-record.md: 577ecc969cd5fef390c8cac5a94a14be2fedc47c907e3ffdb62a57d5a94bb565
- published/confidently-wrong-process-record.html: 5f57e154291ed42d3acdad1dc5b6b3a15694fc35b5d18d06fb873f94b3e56d23

For What a Dead Kid Buys You, at commit e8ad4ed:

- what-a-dead-kid-buys-you/what-a-dead-kid-buys-you-process-record.md: a633971a5b59e2dbceb4028ab88dff67562a4409a5cf62bd99e71119898a36f0
- published/what-a-dead-kid-buys-you-process-record.html: d468ac260a904d3ef0f401d8691ae160263c1899a8fcf788d58e79a07aee7bf5

### Records that are not pieces

The repo also holds receipts about the work itself. Those are anchored too, with a type that says what they are instead of borrowing the fields a published piece uses.

| Record | Topic | Message | Timestamp (UTC) | Version anchored |
|---|---|---|---|---|
| Receipt: the E.D.A.I. shield says "watching." Almost. | [0.0.10897644](https://hashscan.io/mainnet/topic/0.0.10897644) | #10 | 2026-10-29 17:25:32 | commit fa58871 |
| Field Test 001: outreach addendum | [0.0.9376001](https://hashscan.io/mainnet/topic/0.0.9376001) | #8 | 2026-10-29 17:26:24 | commit ece87a2 |

The shield receipt went up as a `work-record`: the same spine as a piece record, without the fields for a published essay, because it documents a build and what that build got wrong.

Field Test 001 has a topic of its own, [0.0.9376001](https://hashscan.io/mainnet/topic/0.0.9376001), because that test is a chain and not a single record. The protocol was pre-registered there on September 30, 2026, before the test ran. On October 13 came the status, an erratum for a harness fix made before any request was sent, a seal for each of the two runs, the analysis code fingerprinted before it had opened the answer key, and a seal over the results themselves, which stay unpublished. The outreach addendum is sequence 8 on that chain, posted as an `erratum`. The files the earlier messages froze were not touched to add it, which is why the addendum is a separate note rather than an edit.

For the E.D.A.I. shield receipt, at commit fa58871:

- edai-shield/edai-shield-record.md: 2622d82b65d27e10ac0645e7b54e641ca223cdfcb4a1cc85aeae5a82884ad49e
- edai-shield/edai-logo.png: 029dff44adfd7359e0947656083ce0a2488088c05b9271ad7a6e78ab1998c5fc

For the Field Test 001 outreach addendum, at commit ece87a2:

- field-test-001/typesafe-outreach-addendum-2026-10-13.md: 4676709bb7362d8d0f9852d03e7df35e4f80f0bc45b60417ee33d94cf4f8277f

## Why

When I was a kid I dictated my schoolwork and felt like a fraud every time the A-plus came back. I'm not hiding the help this time. This is the whole process, open, so you don't have to take my word for it.

If you want to argue about whether this counts as writing, good. That's the conversation I want to have in public.

Gage Woodle
