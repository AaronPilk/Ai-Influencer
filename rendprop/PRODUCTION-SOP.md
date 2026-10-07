# Rendprop AI Hosts — Production SOP

**Method:** Pilk films every clip himself, in real spaces, then Higgsfield Genjutsu swaps him out for Ava or Mia. The house, the light, the camera move and the performance are all real. Only the person changes.

**Status:** v1 — written 7 Oct 2026 before the first test swap. The test clip (see §6) decides the open questions marked ⚠️. Update this file after it runs.

---

## 1. Why this method

- Real locations. Rendprop sells tours of real spaces; the host standing in one is the proof.
- Real gestures and timing. No motion templates, no puppet look.
- The phone-walkthrough demo can be in the same take.
- Zero copyright exposure. Nothing is borrowed from someone else's viral clip.
- One generation per reel if the take is structured right (§4).

## 2. The pipeline

```
MIA (American)
FILM (phone, 9:16)  →  TRIM to ≤ 25 s  →  GENJUTSU OBJECT SWAP (Pilk → Mia)
→  SPEECH-TO-SPEECH (Pilk's track → Mia's voice; timing unchanged)
→  [LIP-SYNC PASS only if the swap's mouth is off]  ⚠️
→  EDIT  →  ZERNIO

AVA (British)
TTS Ava's line first  →  FILM to playback (earbud, say it with her)  →  TRIM
→  GENJUTSU OBJECT SWAP (Pilk → Ava)  →  replace audio with the TTS track
→  VIDEO-TO-VIDEO LIP-SYNC to the TTS (always)
→  EDIT (hook b-roll, demo cutaway, captions, AI-host label, CTA)
→  ZERNIO schedule (Rendprop IG · FB · YouTube Shorts)
```

Why two paths: voice conversion keeps the speaker's accent. Pilk's American delivery can become Mia; it can't become a British Ava. Details in §7.

### Genjutsu settings

| Setting | Value | Why |
|---|---|---|
| Mode | **Object Swap** | Keeps the real room, light and camera. Motion Transfer rebuilds the whole scene from references — wrong tool here. |
| Clip length | 4–30 s hard limit; aim 12–25 s | One take per reel. |
| Identity refs | The host's **3-view reference sheet** (gray seamless) + a chest-up portrait if we make one | Clean refs on a neutral background. Do **not** feed the "motion-start" images with the fictional interiors — they pull that room into the result. |
| Prompt | See §3 | Tag the images with `@` — reports say that measurably improves accuracy. |
| Test resolution | 480p | Cheapest, and reportedly renders in seconds while 720p/1080p queue. Approve the look here. |
| Final resolution | 720p minimum, 1080p for anything we'll run as an ad | Reels get recompressed anyway; 720p is the floor. |

### Credits (third-party figures — the generator shows the real number before you confirm)

| Clip | 480p | 720p | 1080p |
|---|---|---|---|
| ~15 s swap | ~40 | ~104 | ~144 |

Plus plan = 1,200 credits/month. Rough budget: 3 test clips at 480p (~150) + first 3 reels at 1080p (~450–600 at 20 s). Re-check after the test; top up only once the pipeline is proven.

## 3. The swap prompt

Flip of the kit's motion-transfer prompt. Paste, swap the host name, tag the uploaded refs.

```
Keep everything in the video exactly the same — the room, lighting, camera
movement, timing and framing. Replace only the main subject (the man) with
the woman in @Image1 and @Image2. She is Ava: long honey-blonde waves,
blue-gray eyes, ivory short-sleeve knit top, beige tailored trousers,
slim dark brown belt, ivory sneakers, small gold stud earrings. Preserve
her face, hair and wardrobe consistently through the whole shot. Match
the original performance: same gestures, same head movement, same mouth
movement and speech timing. Natural realistic anatomy, clean hands, no
extra fingers, no face drift, no wardrobe changes, no additional people,
no generated text or logos.
```

Mia version: `long espresso-brown blowout with a center part, rich brown eyes, warm olive skin, open violet tailored blazer, ivory square-neck knit top, charcoal trousers, white sneakers, small gold hoop earrings.`

Never put both women in one single-person swap.

## 4. Filming rules (this is what makes or breaks the swap)

**Camera**
- 9:16 vertical, 1080p, **30 fps**. Not 60/120.
- Talking segments: phone fixed — tripod, or propped. Walk-and-talk: slow, smooth, two hands on the phone. The swap keeps your camera motion, so shake in = shake out.
- Frame chest-up for talking, full body for walkthroughs. **Leave headroom and side room** — the host has long hair; give it space.
- Lens at your chest/eye height. Avoid looking down into the phone.

**Light**
- Bright, even daylight. Rooms with big windows are ideal — that's also what Rendprop tours look best in.
- Light on your face, not behind you. Backlit face = mushy face reconstruction.

**You**
- Fitted, plain, mid-tone clothes. No white shirt against white walls, no logos, no hat, no glasses, no hoodie, no baggy anything. The swap re-dresses you from the wardrobe reference; a clean silhouette helps it.
- Hands visible, deliberate, below the shoulders. Don't touch your face or hair. No fast flicks or pointing at the lens — hands are where swaps fall apart.
- Holding the phone up to "film" is fine if it stays steady. Don't pass objects hand to hand.
- Speak a touch slower and more articulated than normal. Your mouth drives her mouth. Her voice will be converted from your track, so clean delivery matters.
- Perform in character. Speech-to-speech keeps your cadence: Ava takes are warm and quick with a smile; Mia takes have a half-beat pause after the joke and a flat delivery.

**The room**
- **Mirrors and glass.** Bathroom mirrors, glass doors, dark TV screens, oven doors — your reflection will show up unswapped. Check the frame for reflections before every take.
- No other people, no pets in frame.
- One continuous take per reel, 12–25 seconds. Two takes of each. Say the script number at the top of each take (trimmed later).

**Audio**
- Quiet room, AC off, phone mic is fine; a lav mic is better. The track gets voice-converted, so room echo becomes her room echo.

## 5. Reel structure — one swap per reel

```
0:00–0:02  HOOK B-ROLL  — the Rendprop result (the fly-through) + on-screen hook text.
            Not you. No swap needed. This is the thumb-stopper.
0:02–0:20  HOST TAKE    — your one continuous take, swapped to the host.
            Her audio runs the whole way through.
0:08–0:15  DEMO CUTAWAY — cut to real app footage while her voice continues.
            Full-screen, 5–8 s, then back to her.
0:18–0:20  CTA          — she says the keyword line; on-screen text matches.
```

One take, one swap, one voice conversion. The demo cutaway and the hook b-roll are edits, not generations.

## 6. The test (do this before the first reel)

Three 8–10 second clips, same day, same room:

1. **Talking, fixed camera, chest-up.** You say a Mia line with a deadpan pause. → Tests face, lips, hair, and Mia's speech-to-speech conversion.
2. **Walk-and-talk, full body, slow handheld.** Walking toward a window saying an Ava line **to playback** (her British TTS in one earbud). → Tests body swap across a gender/build difference, feet, camera motion, and the Ava TTS + lipsync path end to end.
3. **Phone in hand.** Chest-up, holding your phone up as if capturing the room. → Tests hands + prop.

Do the voice design (§7.1) **before** this shoot so clip 2 has a real Ava line to play back.

Render all three at 480p. What to check:

- ⚠️ **Is the source audio preserved in the output?** If not, we keep your original track and lay the converted voice over the swapped video.
- ⚠️ **Do her lips track your speech?** Good enough → voice change only. Mushy → add a lip-sync pass using the converted audio.
- Face consistency between clip 1 and clip 2 (same woman?).
- Hands in clip 3.
- Hair behavior when you turn your head.
- Any reflections or ghosting.

Pass → render the first reel at 1080p. Fail on lips → lip-sync pass. Fail on identity → add a chest-up portrait to the refs and re-test. Then update this file.

## 7. Voices — Ava is British, Mia is American (decided 7 Oct 2026)

**The constraint that shapes this:** speech-to-speech voice conversion keeps the *source speaker's accent*, cadence and emotion and only swaps the timbre. ElevenLabs documents it plainly — record American, pick a British voice, you get the British voice with an American accent. Higgsfield's Voice Change is the same class of tool. So:

| Host | Accent | Audio path | Lip-sync pass |
|---|---|---|---|
| **Mia** | General American | **Speech-to-speech** from Pilk's take → Mia's voice. Timing identical to the swap, lips already match. | Only if the swap test shows mouth drift |
| **Ava** | Modern southern English (light, not posh) | **Text-to-speech** in Ava's designed voice. Pilk films to playback (below). TTS track replaces his audio. | **Always** — video-to-video lipsync (Kling Lipsync / Sync Lipsync 3 in Higgsfield's Lipsync Studio) locks her mouth to the TTS |

### 7.1 Design the voices once (ElevenLabs Voice Design — describes a voice into existence; no real person is cloned)

Generate three candidates per description, pick one by ear, save it with the host's name, never regenerate. Export a 30-second sample of each as the reference. Paid plan = commercial rights.

**What we learned on 7 Oct (first live session):** the "clean studio recording, perfect audio quality" style of prompt produces an announcer — Pilk's verdict was "sounds like AI too much." The fix that worked, in his words "much better": describe a *real person in a real situation*, ask for imperfection, turn **Generate Preview Text OFF** and paste an actual conversational script line with a `[laughs]` tag, and drop **Guidance Scale to ~18%** (default was ~38%). Loudness left at default.

**Ava — the prompt that worked:**
> A real young woman from the south of England, late twenties, recorded casually like a voice note to a friend. Modern everyday southern English accent, not posh, not newsreader, not theatrical. Warm, playful, a bit cheeky, quick and bright with a natural smile in her voice. Imperfect and human: uneven pacing, small breaths, light natural room tone, the occasional soft laugh. Mid register. Sounds like a mate explaining something she's excited about, never like an advert or an announcer.

Preview text used: *"Okay so... this room has potential. Right now the floor's doing all the work. [laughs] Rendprop's photo studio drops furniture in, so buyers can actually picture living here. And it keeps the original right next to it, labelled, so nobody's getting fooled. Honestly? Brilliant. Comment STAGE and I'll send you the app."*

**Mia — same recipe:**
> A real American woman, early thirties, recorded casually like she's talking to a friend across a table. General American accent. Calm, confident, dry sense of humor — lands a joke without smiling. Slightly lower register, even unhurried pace, understated. Imperfect and human: natural breaths, light room tone, a half-beat pause before the punchline. Never salesy, never an announcer.

Preview text: *"I filmed this whole house on my phone. Took four minutes. [pause] Rendprop turned the walkthrough into a tour that scrolls like a movie. Tap a room, jump straight to it, send one link. No photographer. No scheduling. No Tuesday. Comment TOUR and I'll send you the app."*

Mia's designed voice only has to be a good *timbre* — her performance comes from Pilk's takes via speech-to-speech, which is why she will always sound more human than any TTS preview.

**SAVED 7 Oct 2026 (ElevenLabs, Creator plan, 30 custom-voice slots):**
- `Ava - Rendprop host (British)` — labels English / British. Pilk picked Voice 1 of the realism batch.
- `Mia - Rendprop host (American)` — labels English / American. Pilk picked Voice 3.
- Never regenerate these. Any "new Ava" is a different woman.

**TTS model for Ava's lines:** Eleven v4 (launched Oct 2026; free on the account for two weeks at kickoff, ~242K credits). Default stability (Natural, mid) and similarity ~75% produced two 21-second takes of the Reel 2 line on the first try. Use `[laughs]`-style audio tags sparingly; write in fragments and ellipses the way people talk.

**AVA LOCKED — 7 Oct 2026.** Pilk heard the Reel 2 line on Eleven v4 and said "she sounds real to me." The designed voice stays; no library swap. Reel 2 and Reel 3 lines are generated and sitting in ElevenLabs History (two takes each, ~20 s) — these are the playback tracks for the test shoot.

Fallback kept on file only: `Charlotte - Warm, Clear, Modern` (library, real recorded British woman, 84K users) if a future line ever reads as AI. Last resort: Ava goes American and runs through Pilk's performance like Mia.

Why that British accent: a light modern southern English voice reads premium and is instantly clear to American ears. Heavy regional accents cost comprehension with a US real-estate audience; stiff RP fights Ava's playful character. If you want her younger and more casual, ask for "Estuary / London" instead.

If you'd rather keep audio inside Higgsfield: upload the ElevenLabs sample to Higgsfield Audio → clone it as a reusable voice there. Higgsfield's own voice creation clones from a sample; it doesn't design from a description.

### 7.2 Mia takes — speech-to-speech

1. Trim your take. 2. ElevenLabs Voice Changer (or Higgsfield Audio → Voice Change): source = your audio, target = Mia. "Remove background noise" on. Stability ~50, similarity ~80, style 0. 3. Lay the converted track under the swapped video — same length, same timing, nothing to align. 4. Loudness-match in the edit.

Perform Mia on set: flat delivery, the half-beat after the joke. Whatever you do with your voice, she does.

### 7.3 Ava takes — TTS + film to playback

1. **Before the shoot**, generate Ava's lines as TTS (ElevenLabs, model v3 or Multilingual v2; stability ~45–55 for expressiveness, similarity ~75, style low). Listen; regenerate until the read is right. Export MP3.
2. **On set**, play her line in one earbud and **say the words out loud with her**, matching her pace. Your gestures, head movement and emphasis now land on her beats. (Standard music-video playback technique.)
3. Swap as normal. In the edit, mute your track and lay her TTS under the swapped clip, aligned to your first word.
4. Run the clip through video-to-video lipsync with her TTS audio. Her mouth now matches her voice exactly.
5. Fallback if you can't do playback on a given shoot: film normally, swap, lipsync to the TTS anyway — the lipsync model re-animates the mouth regardless. You lose a little gesture-to-word alignment, nothing more.

### 7.4 Writing for a British Ava

The audience is American agents and owners, so **keep US real-estate vocabulary** (listing, agent, photographer, open house). Let her *phrasing* be lightly British — "brilliant," "sorted," "a bit," "lovely" — one per script at most. Never "estate agent," "flat," or "viewing"; those confuse the buyer we're talking to.

### 7.5 Cost

ElevenLabs Creator plan (~$22/mo) covers a month of reels many times over — 30 reels × 20 s is about 10 minutes of audio. Lipsync passes cost Higgsfield credits; the generator shows the number. Budget roughly one extra lipsync per Ava reel on top of the swap.

## 8. Edit spec

- 9:16, 1080×1920, 30 fps, ≤ 20 s for the first series.
- Captions: large, high-contrast, in the safe zone (away from the bottom 20% and the right-side controls).
- On-screen ID in the first 2 seconds of the host appearing: **"Ava · Rendprop AI host"** / **"Mia · Rendprop AI host."**
- Demo cutaways use real app recordings and real hosted tours only. AI-staged photos show the original next to the result with an "AI virtually staged" label. The sample houses in the app are labeled "AI demo property."
- Brand: violet #7C3AED on ink #0B0D10 / paper #F2F3F5 for text plates. Rendprop mark on the CTA frame only.

## 9. Publishing

- Account: the existing Rendprop Instagram, cross-posted to Facebook and YouTube Shorts via the Zernio setup already wired for the carousels. TikTok is awareness only (AI content is barred from Creator Rewards and suppressed when labeled).
- **Turn on Instagram's "AI-generated profile" label** before the first host reel goes up. Labeled accounts take no reach penalty; unlabeled ones do.
- Caption always carries the disclosure line and the keyword CTA (see FUNNEL.md).
- Cadence target once the pipeline is proven: one reel a day, batch-filmed weekly (ten takes in one shoot = a week and a half of content).

## 10. Legal / brand lines we don't cross

- Neither host is ever presented as a licensed agent, a customer, the founder, or the subject of a success story.
- No pricing, trial or "free" claims in the videos — those live in the app and change.
- No guarantees about lead volume, speed or sales. "Capture quality affects the finished tour" is fine to say.
- Listing media shown in demos never contains AI-rendered people. The host talking to camera is not listing media.
