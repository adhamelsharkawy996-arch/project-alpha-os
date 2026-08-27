# Project Alpha — Locked Audio Voice

## THE VOICE (locked 26 Aug 2026 by Adham)

```
Name:      Omarii - Persuasive Outbound
voice_id:  hYqZq4J77gUOQZK4uSvg
accent:    egyptian
gender:    male
age:       young
platform:  ElevenLabs (Creator tier, commercially licensed)
```

**Chosen after blind audition of 6 Egyptian-accent voices on a real Project Alpha script.**
Adham's verdict: *"the best with the correct narration and speaking letters"* — i.e. correct
Masri pronunciation and clean articulation, no MSA drift.

## Locked generation settings

```json
{
  "model_id": "eleven_multilingual_v2",
  "voice_settings": {
    "stability": 0.5,
    "similarity_boost": 0.75,
    "style": 0.35,
    "use_speaker_boost": true
  }
}
```

Do not change these without a fresh A/B against the audition sample.

## Measured timing (use for script budgeting)

| Chars | Duration |
|---|---|
| 187 | 15.2s |

**≈ 12.3 characters per second.**
For an 18-20s reel: **220-250 Arabic characters.** Overrunning is the most common mistake.

## Reference audition sample

`~/projects/reels/voice-audition/Omarii_persuasive.mp3` (15.2s)
Script used:
> موقعك شكله حلو… بس هل بيساعدك تبيع؟ في Project Alpha Tech إحنا مش بنعمل مواقع شكلها حلو وبس. إحنا بنعمل مواقع بتفهم عميلك، وبتشتغل ٢٤ ساعة عشان تجيبلك بيزنس. عايز موقع بيبيع فعلاً؟ كلمنا.

Keep this file as the regression baseline. If output ever sounds different, compare against it.

## Rejected candidates (do not re-litigate without reason)

| Voice | voice_id | Note |
|---|---|---|
| Ziad - Dynamic and Vibrant | 5REPlS2Ja1VZ7zNA0ykn | energetic, not chosen |
| Mostafa - Bold and Spirited | QvNF0qyyt1Tuy1YAmnzH | punchy, not chosen |
| Mamdoh - Deep Egyptian | 68MRVrnQAt8vLbu0FCzw | most-used on platform, not chosen |
| Hazem - Confident News Presenter | BEK0cM5ocuhluB2yKvMa | too broadcast/formal |
| Fattah | UDyuvKjPXutvqdCvJ0Oh | neutral, not chosen |

## Usage notes

- Cache generated audio by script hash. Never re-bill for an unchanged script.
- Use `POST /v1/text-to-speech/{voice_id}/with-timestamps` for caption sync.
- Validate `alignment.character_start_times_seconds` before rendering — known ElevenLabs
  issue (#760) where values can collapse to identical. Abort and re-request if non-monotonic.
- Group characters into WORDS for animation. Never animate per-character (Arabic is cursive).
