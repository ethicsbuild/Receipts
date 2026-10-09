# Receipt: The E.D.A.I. Shield Says "Watching." Almost.

**Record date:** October 8, 2026
**Principal:** Gage Cass Woodle
**Prepared by:** Lumen (a Claude instance, Anthropic)
**Status:** Published October 8, 2026, as read and approved by the principal. Not yet anchored on Hedera.

---

## What this record is

The E.D.A.I. logo is a gold shield with three lines of binary inside an eye. The intent was for the code to say "watching": the project watches the technology. This record documents what the code actually says, how the error got through, and how it was caught. Nothing in it has been corrected after the fact. The logo is staying up as it is.

## The artifact

- **File:** `edai-logo.png`, served at edai.quest, source in the public repo `ethicsbuild/edai-landing` at `public/edai-logo.png`. A copy sits next to this record as [edai-logo.png](edai-logo.png).
- **SHA-256:** `029dff44adfd7359e0947656083ce0a2488088c05b9271ad7a6e78ab1998c5fc`
- **Code as it appears in the image:**

```
01100100
00110010
01000116
```

## What the code was meant to say

The design has two layers.

1. **Binary to characters.** Each line is eight bits that stand for one character.
2. **Characters to Base64.** The characters are the start of the word "watching" encoded in Base64, a standard way of turning text into a string of safe characters.

"watching" in Base64 is `d2F0Y2hpbmc=`. Decoding `d2F0Y2hpbmc=` gives back "watching." Both directions were checked by running them in code on October 8, 2026.

## What it actually says

| Line | Decodes to | Status |
|---|---|---|
| `01100100` | d | valid |
| `00110010` | 2 | valid |
| `01000116` | none | **invalid.** Binary uses only 0 and 1. This line contains a 6. |

Two failures stack:

- **Truncation.** Even if every line were valid, three characters (`d2F`) are only the first three of the twelve in `d2F0Y2hpbmc=`. The shield never had room for the whole word.
- **Corruption.** The third line was meant to be `01000110` (F). The image has `01000116`. The image was most likely made by an AI image generator, and these tools are known for drawing text and code that look right but aren't. That cause is a likely explanation, not a confirmed one.

## How it got through: the first check

On July 15, 2025, the principal gave the shield to Claude and asked what the code said (chat titled "Binary Code Decoding Challenge," later shared as "EDAI Logo Mystery").

Claude transcribed the third line as `01000110`. That is not what the image shows. It then decoded a clean "d2F," suggested it might be part of a Base64 string, and asked whether it belonged to a larger puzzle.

It never said the third line wasn't valid binary. It quietly read the broken digit as the digit that fits, and reported a clean result. That's the pattern E.D.A.I. was built to catch: a confident, tidy answer with no note of what it smoothed over. The flaw then stayed on the shield for more than a year.

## How it was caught: the second check

On October 8, 2026, the principal said the shield's code "is supposed to spell out watching." Instead of accepting that, Lumen downloaded the logo from the public repo, read the code from the image, and decoded each line in code. The result:

- Lines 1 and 2 are valid. Line 3 raises an error (`invalid literal for int() with base 2: '01000116'`).
- The first conclusion was "it doesn't say watching." That turned out to be incomplete.
- After the principal pointed to the July 2025 chat, the "d2F" result led to the Base64 layer, and the design's intent was confirmed.

The second check was also nearly confidently wrong. "It doesn't say watching" was true of the image and false about the design. It took the principal's own record to correct it.

## Findings

1. The design intent was sound: binary, then Base64, then "watching."
2. The artwork cut the message to 3 of 12 characters and corrupted one of them.
3. The first AI check silently fixed the corruption instead of reporting it.
4. The second AI check caught the corruption but missed the design until the human's record filled the gap.
5. No fix is applied. The logo stays as it is, as evidence.

## The principle

A machine that can't say "I don't know" will say something else instead. In July 2025 it said "d2F." The honest answer was "two of these lines are valid and the third isn't binary at all."

## Verification anyone can repeat

```python
import base64
for b in ["01100100", "00110010", "01000116"]:
    try: print(b, "->", chr(int(b, 2)))
    except ValueError: print(b, "-> not valid binary")
print(base64.b64encode(b"watching").decode())   # d2F0Y2hpbmc=
```

Hash the logo file and compare it to the SHA-256 above to confirm it's the same image.
