# VideoExpress Hindi Devotional-Moral Cartoon Agent

A system prompt for producing Hindi kids' moral-story cartoon videos in VideoExpress.ai, in the style of Indian 2D devotional cartoons: chibi children, gentle elders, pastel painted worlds, simple Hindi dialogue spoken by on-screen characters (no narrator) and a clear moral. It replaces the earlier stickman narrated-story workflow and the desi-comedy workflow in the older repository.

Style direction comes from a visual study of the reference video https://www.youtube.com/watch?v=SYkEN_3n3PI (see STYLE_BIBLE.md for what was and was not observed). Characters, stories, lines and designs are original and must never copy that channel.

## What changed from the earlier workflows

| Topic | Stickman agent | Desi comedy agent | This agent |
| --- | --- | --- | --- |
| Character look | Plain 2D stickman | Caricature cartoons, thick outlines | Chibi children with huge glossy eyes plus slim gentle adults, soft rounded outlines |
| Backgrounds | Simple fixed locations | Painterly textured sets | Pastel painted worlds: skies, pillars, mountains, village courtyards, rivers |
| Story | Calm narrated story | Joke-dense "every Indian ___" gags | Moral story: hook, trouble, effort, turning moment, change of heart, moral, final gag |
| Voice and lipsync | One cloned narrator voice | Characters speak their lines | Characters speak simple Hindi at a normal pace; no narrator, every line comes from a character on screen; Advanced Mode, not Lipsync HD |
| Clip length | 3–5 seconds | 7–10 seconds | 7–10 seconds, about 44–48 clips for 6 minutes |
| Subtitles | None | Optional editor text layer | Hindi two-line editor text layer plus optional channel watermark, never drawn by the video model |
| Tone | Calm | Fast, slangy | Warm, respectful, family-friendly |

## Use

1. Open SYSTEM_PROMPT.md and paste the whole prompt into Claude or another browser-capable agent.
2. Enable its supported browser control and keep production visible. Sign in to VideoExpress yourself.
3. Send a topic or moral, or point at the sample script, as shown in examples/example-request.md.
4. The agent builds characters, references, clips, the timeline, then saves and exports.

## Contents

- SYSTEM_PROMPT.md — the production agent prompt
- STYLE_BIBLE.md — what the reference video looks like and how to reproduce it
- examples/example-request.md — paste-ready requests
- examples/story-mitti-ki-ghanti.md — an original 46-clip Hindi script "मिट्टी की घंटी" with cast, set layouts, narration and sample prompts
- examples/story-jai-jagannath-chhote-bhakt.md — an original 46-clip Hindi Rath Yatra script "जय जगन्नाथ | रथ यात्रा में छोटे भक्त का चमत्कार" with a respectful-depiction rule, cast, set layouts and sample prompts
- evals/acceptance-checklist.md — production acceptance checklist

## Known limits

- VideoExpress clips sometimes carry burned-in garbled captions. The prompt never mentions text and every clip is checked.
- Only two Reference Photo slots exist, so scenes with three or more people use group reference images.
- Audio could not be heard during the reference study, so voice and accent guidance is based on captions and mouth shapes.
- The video model may move the mouths of non-speakers or add extra people; every clip is checked.

## Security

Never put passwords, tokens, API keys, payment data or browser session data in this repository.
