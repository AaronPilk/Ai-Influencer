# Rendprop Hosts — Asset Registry

IDs that can be reused in Higgsfield generations without re-uploading. Media IDs are permanent in the workspace; job IDs can be passed as reference media too.

## Higgsfield media (uploaded 7 Oct 2026)

| Asset | media_id | Notes |
|---|---|---|
| Mia — 3-view reference sheet | `65e613b6-44ed-4fd9-91c6-10e832c0a22a` | Gray seamless; identity ref |
| Mia — full-body motion-start (fictional entry hall) | `c64f3616-aea3-4ac8-9741-13d949213c20` | Identity/wardrobe ref; its room is NOT the target scene |
| Test clip 1 — Pilk, apartment, 0:00–0:29.2 of IMG_7268.mov, 1080×1920 @ 30 fps | `815a711f-722e-4db4-9c3d-fda31df39ca6` | Source performance for the first swap |
| Clip 2 — Pilk, real townhome across the street, 0:14.3–0:37.7 of IMG_7271.mov (23.4 s), 1080×1920 @ 30 fps | `f8b44df9-56d9-4b96-b592-71db5b992888` | Waist-up, handheld, overcast. First Object Swap source |

| Ava — 3-view reference sheet | `e797cdc5-0d80-4b92-903f-5e2bcbb560bc` | Gray seamless; identity ref |
| Ava — full-body motion-start (fictional living room) | `8ca75c6f-2870-4766-971d-bb8062212e24` | Identity/wardrobe ref; its room is NOT the target scene |

## Higgsfield generations

| What | job_id | Model / settings | Credits |
|---|---|---|---|
| Listing exterior — modern white coastal Florida home, 9:16, no people | `26d41d66-f9c5-4723-a7a4-9dfbac2e4e1b` | gpt_image_2_5 | — |
| **Test 1 — Mia, motion transfer, placed in front of the listing exterior** | `0d20abe4-caab-4b62-86bf-16e476728161` | hf_mult_motion_control, 480p, 29.2 s | **87** |
| **Test 2 — Ava, same source + plate, grounding/shadow prompt** | `83adf5be-b61f-4bf6-98ad-165cd836446b` | hf_mult_motion_control, 480p, 29.2 s | **87** |
| **Clip 2 — Ava, OBJECT SWAP on the real townhome footage (background kept)** | `4ac1fdef-1e43-41c0-9491-05665672a11b` | hf_mult_replace_object, **1080p**, 23.4 s | **264** (720p would have been 168) |

## ElevenLabs conversions of the test-1 audio (29.2 s)

| File | Voice | Source | Settings | Verdict |
|---|---|---|---|---|
| `ElevenLabs_2026-10-07T17:07:12_Mia…` | Mia | original pitch | s50 / sb75 / se0, noise removal | "sounds deeper" |
| `ElevenLabs_2026-10-07T17_11_33_Ava_…_sp100_s50_sb75_se0_b_e2.mp3` | Ava | **+4 semitones** | s50 / sb75 / se0, speaker boost | **"sounds good" — chosen for the test clip** |
| `ElevenLabs_2026-10-07T18:19:33_Ava…_sp100_s50_sb75_se0_b_e2.mp3` | Ava | clip 2 audio, **+4 semitones** | s50 / sb75 / se0, noise removal, speaker boost | for the townhome clip — pending mux |

## Real costs observed

- Motion transfer (`hf_mult_motion_control`), 29.2 s source, 480p → **87 credits**. ~3 credits/s at 480p.
- Object swap (`hf_mult_replace_object`), 23.4 s source → **168 credits at 720p, 264 at 1080p** (~7.2 and ~11.3 credits/s). Budget ~11 credits per second for a 1080p final.
- Higgsfield balance after the clip-2 submit: ~705 of the 1,200 monthly Plus credits.
- ElevenLabs speech-to-speech: ~486 credits per 29 s (≈17/s) on Creator.

## ElevenLabs voices (Creator plan)

- `Ava - Rendprop host (British)` — designed voice, Eleven v4 for TTS
- `Mia - Rendprop host (American)` — designed voice, used as the speech-to-speech target

## Source footage

- `IMG_7268.mov` — 41 s, 4K/60, portrait (rotation −90), shot in Pilk's apartment, freestyle script (transcript in SHOT-LIST notes). Lives in `~/AI influencer/` on his Mac. Segment 0:29–0:41 ("book views… it's insane") is unused so far.
