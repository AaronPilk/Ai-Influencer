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
FILM (phone, 9:16)  →  TRIM to ≤ 25 s  →  GENJUTSU OBJECT SWAP (Pilk → Ava/Mia)
→  VOICE CHANGE (Pilk's track → host voice, speech-to-speech)
→  [LIP-SYNC PASS only if the swap's mouth is off]  ⚠️
→  EDIT (hook b-roll, demo cutaway, captions, AI-host label, CTA)
→  ZERNIO schedule (Rendprop IG · FB · YouTube Shorts)
```

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

1. **Talking, fixed camera, chest-up.** You say a Mia line with a deadpan pause. → Tests face, lips, hair, voice conversion.
2. **Walk-and-talk, full body, slow handheld.** Walking toward a window saying an Ava line. → Tests body swap across a gender/build difference, feet, camera motion.
3. **Phone in hand.** Chest-up, holding your phone up as if capturing the room. → Tests hands + prop.

Render all three at 480p. What to check:

- ⚠️ **Is the source audio preserved in the output?** If not, we keep your original track and lay the converted voice over the swapped video.
- ⚠️ **Do her lips track your speech?** Good enough → voice change only. Mushy → add a lip-sync pass using the converted audio.
- Face consistency between clip 1 and clip 2 (same woman?).
- Hands in clip 3.
- Hair behavior when you turn your head.
- Any reflections or ghosting.

Pass → render the first reel at 1080p. Fail on lips → lip-sync pass. Fail on identity → add a chest-up portrait to the refs and re-test. Then update this file.

## 7. Voices (one-time setup, after the test says which path we need)

- Create **two** voices, once. Ava: warm, bright, conversational American English, mid register. Mia: calm, slightly lower, dry. Save both; never regenerate them.
- Speech-to-speech conversion of your take (not text-to-speech) — it keeps your timing so the lips stay honest.
- Loudness-match every clip in the edit; converted voices come out at inconsistent levels.

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
