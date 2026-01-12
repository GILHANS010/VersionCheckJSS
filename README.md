# Update Log

Hello, this is **QLAUDIO**.  
We would like to inform you of the latest updates for the **Josun Series**.

- New update information will be announced after the update has been completed.
- If you are using a version older than the latest one listed below, please re-download using the purchase email link we sent you to receive the updated version.
- If you discover an issue even though your installed version is already newer than the listed version, please contact us at **contact@qlaudio.com** and we will resolve it promptly.
- If the download link does not reflect the latest update, or if you have any other inquiries, please contact us at the same email address.

Thank you.  
Sincerely,  
**QLAUDIO**

---

## Added: Update Check File (`checkVersion.html`)

Starting from **v1.5.1**, the file `checkVersion.html` is automatically included in the folder.

- When executed, it compares your current installed version with the latest version on the server and indicates whether an update is required.
- When updating the Josun Series, you must re-download **`checkVersion.html`** together for it to work correctly.
- If the file is missing, please download `checkVersion.html` separately using the link in your original purchase email.

---

## Update History (Current Latest Version: **1.12.1**)

---

### v1.12.1 (2026.01.12) — Nabal & Nagak: Velocity Layers Added & Sound Expanded

- **Nabal & Nagak Library Update:** Added new audio samples to the Nabal and Nagak libraries.
- **Velocity Layers Applied:** Implemented velocity layers to allow sound character to change based on playing strength, resulting in a much richer and more realistic sound.

---

### v1.12.0 (2025.12.15) — Library Integration, Instrument-Group Guides Added, Manual Updated

#### RoundRobin & NoRoundRobin Library Integration
- The previously separated **RoundRobin (Default)** library and **NoRoundRobin** library have been merged into a single library.
- After entering an instrument, you can choose:
  - **RoundRobin (Default):** natural variation per hit/note
  - **NoRoundRobin:** fixed samples
- **Applied libraries:** `Jangdan`, `Samulnori (Heritage)`, `Samulnori (Modern)`

#### Mono & Poly Library Integration
- The previously separated **Mono (monophonic)** and **Poly (polyphonic)** libraries have been merged into a single library.
- After loading an instrument, you can select **Mono/Poly** directly within the interface.
- **Applied libraries:** `Ajaeng (Jungak)`, `Ajaeng (Sanjo)`, `Haegeum`, `Danso`, `Daegeum (Jungak)`, `Daegeum (Sanjo)`,  
  `Daepiri`, `Hoon`, `Jeog`, `Ji`, `Nabal`, `Nagak`, `Piri (Dang)`, `Piri (Hyang)`, `Piri (Se)`,  
  `So`, `Sogeum`, `Taepyeongso`, `Tungso`, `Yak`

#### Added Instrument-Group Detailed Guides (`README.html`)
- Added `README.html` files in each folder:
  - **Woodwinds**
  - **Strings**
  - **Percussion**
- Running the file provides detailed information such as:
  - Playing methods (**Key Switches**)
  - **Key Mappings**
  - **CC controller** functions
- Default language is **English**; you can switch to **Korean** using the top button.

#### Manual & EULA Update
- Updated documents for clearer feature descriptions and explicit license terms (**EULA**).
- Supports **Korean / English**.

---

### v1.11.5 (2025.11.28) — Size Optimization for Strings & Woodwinds

- Optimized sample data to reduce library size **without quality loss**.

**Size reduction**
- Strings series: ~ **120 MB**
- Woodwinds series: ~ **740 MB**

> Note: This update only optimizes file size and does not change functionality or sound.  
> If your current version works fine, updating is optional. Update only if you need to free up storage.

---

### v1.11.4 (2025.11.05) — Percussion Manual Update & Cinematic Note Fixes

#### Percussion Manual (All) Review & Revisions
- **Fixed octave notation error:** A mix-up between **Concert Pitch (C1=24)** and **Computer programming standard (C2=36)** caused the percussion manuals (including Cinematic) to be written **one octave higher** than actual. This has been corrected.  
  - Example: `Chuk D7 -> D6`
- **Added missing information:** Added missing instrument placement info for the **Temple & Ritual** library.

#### Cinematic Library: Partial Note Mapping Changes
- Updated some notes for more natural performance:

- `A#4 (70) ~ D5 (74) : Yeonggo`  
  → `A#4 (70) ~ D#5 (75) : Yeonggo`

- `D#5 (75) ~ F#5 (78) : Bak`  
  → `E5 (76) ~ F#5 (78) : Bak`

- `A6 (93) : Nodo`  
  → `A6 (93) ~ A#6 (94) : Nodo`

---

### v1.11.3 (2025.08.13) — Added “Temple & Ritual” Library (Percussion)

- Added **Temple & Ritual** library to the **Percussion series** and **Platinum Bundle**.  
  This library includes spiritual and ritual percussion sounds used in **Buddhist ceremonies** and **shamanistic rituals (gut)**.

**Main included instruments**
- Buddhist bell / temple bell: from small ritual bells to large temple bells with deep resonance
- Drum: powerful heartbeat-like drum sounds central to rituals
- Jing (large gong): deep, wide resonance often signaling the start of jangdan
- Moktak (wooden fish): clear sound used to keep rhythm during chanting
- Hand bells, Jeongju, Yoryeong, etc.: bright, spiritual metal percussion instruments

---

### v1.11.2 (2025.08.05) — Fixed Percussion NoRoundRobin Bug

- Fixed a bug where samples could play duplicated in some situations in certain **NoRoundRobin** percussion libraries.

**Patched libraries**
- `Jangdan (NoRoundRobins)`
- `Samulnori (Heritage) (NoRoundRobins)`
- `Samulnori (Modern) (NoRoundRobins)`

---

### v1.11.1 (2025.07.02) — Added Nabal & Nagak (Woodwinds / Platinum Bundle)

- Added **Nabal** and **Nagak** libraries to the **Woodwinds series**.
- Although both instruments produce only a single pitch in reality, for usability they were implemented to play **all notes within one octave**.

**Nabal**
- Brass instrument made from long metal, producing a deep, resonant single tone (similar to a trombone).
- No finger holes; used in **daechwita (military ceremonial music)** to create a solemn atmosphere or send signals.

**Nagak**
- Natural instrument made from a large conch shell.
- Deep, majestic foghorn-like sound; produces a single sustained tone and adds a mysterious, solemn atmosphere in daechwita and similar contexts.

---

### v1.11.0 (2025.06.04) — Added Keyswitch On/Off (All Woodwinds & Strings)

- Added a new **“Keyswitch”** button in the UI.
- You can toggle keyboard-based articulation switching (**Keyswitch**) on/off in real time.

**Behavior**
- **Keyswitch ON (Default):**
  - Works as before; press specific keys to switch articulations.
  - Keyswitch keys are visually indicated on the UI keyboard.
- **Keyswitch OFF:**
  - Keyswitch-designated keys behave like normal playable keys (if samples are mapped) or do nothing.
  - Articulations can be changed only via the UI dropdown.
  - Keyswitch color indicators disappear.

**Applied libraries**
- **Strings:** Gayageum (Jungak, Sanjo, 25-string), Geomungo (Jungak, Sanjo), Ajaeng (Jungak, Sanjo), Haegeum  
- **Woodwinds:** Daegeum (Jungak, Sanjo), Sogeum, Junggeum, Danso, Tungso, Saenghwang, Taepyeongso,  
  Hyangpiri, Sepiri, Dangpiri, Daepiri, Ji, Yak, Jeog, Hoon, etc. (all woodwinds with existing keyswitch support)

**Benefit**
- Prevents unintended keyswitch inputs during complex sequencing, or lets you use the keyswitch range as playable keys in certain contexts.

**UI / Stability**
- Minor layout/readability improvements (where applicable).
- Improved stability/responsiveness of keyswitch via internal script optimization.

---

### v1.10.0 (2025.04.30) — Convolution Reverb Type Selection + Manual Update

#### Added IR Type Selection (Dropdown)
- Options:  
  `cathedral.wav` / `chamber.wav` / `dream.wav` / `hall.wav` / `large_hall.wav` / `outdoor.wav` / `plate.wav` / `room.wav` / `studio.wav`
- Default: `hall.wav`

#### Reverb Type Descriptions
- **Cathedral:** vast space, rich lows, grand/mysterious
- **Chamber:** soft, warm, intimate indoor feel
- **Dream:** subtle, translucent tail; dreamy/ethereal
- **Hall:** balanced reflections; natural spaciousness
- **Large Hall:** wide, lush stage-like reflections
- **Outdoor:** open-air diffusion; fresh, open feel
- **Plate:** bright, shimmering reflections; crisp resonance
- **Room:** cozy, realistic early reflections; intimate
- **Studio:** subtle reflections only; clean depth

#### Manual Update
- Added documentation for IR type selection.
- Expanded explanation of Percussion RoundRobin / NoRoundRobin.
- Misc. typo and wording improvements.

---

### v1.9.9 (2025.04.08 09:24) — Added Percussion NoRoundRobin Libraries

- Added **NoRoundRobin** libraries for:
  - `Jangdan`
  - `Samulnori (Heritage)`
  - `Samulnori (Modern)`

**Round Robin**
- A feature that plays different sample variations each hit to increase realism.

**Pros**
- Reduces artificial repetition by triggering different samples for the same note.

**Cons**
- If you need the exact same sample each time, it can be unnecessary.

- Added NoRoundRobin libraries to provide broader user choice.

---

### v1.9.8 (2025.04.02 12:58) — Fixed Jangdan “Byeonjuk Triplet” Sample Resource

- Fixed an issue where silence at the start of the byeonjuk triplet sample caused delayed playback.

---

### v1.9.7 (2025.03.14 14:50) — Optimized Convolution Reverb Default Mix (All Libraries)

- Updated Convolution Reverb mix default:
  - **0.30 (30%) → 0.15 (15%)**
- Based on feedback that the previous default was too strong; changed after testing.

---

### v1.9.6 (2025.03.02 13:12) — Added Per-Instrument Volume & Panning Knobs (Samulnori)

- Updated `Samulnori (Modern)` and `Samulnori (Heritage)`
- Added per-instrument **Volume** and **Panning** knobs  
  (e.g., Janggu, Kkwaenggwari), enabling more precise mixing and sound design.

---

### v1.9.5 (2025.02.19 14:41) — Added Delay Time Knob + Fixed Geomungo Sanjo (Poly) Voice Error

#### Added Delay Time Control Knob
- Added a knob to directly control delay time.
- **Time Sync:** follows DAW BPM automatically
- **Musical values:** selectable in musical time units (e.g., 1/16, 1/4 notes)
- **Real-time response:** immediate reflection for intuitive sound design

#### Fixed Geomungo Sanjo (Poly) Voice Error
- Fixed an issue where vibrato notes would sound simultaneously in the Basic playing method.

---

### v1.9.4 (2025.01.22 13:05) — Portamento Glide Time Revision

- Improved Portamento behavior:
  - More natural glide-time control
  - More delicate mid-range control, larger changes in later range
  - Optimized response curve
  - Fixed abrupt/unexpected behavior from previous versions

---

### v1.9.3 (2025.01.06 15:23) — Added Jangdan & Samulnori (Heritage); Renamed Samulnori

- Added 2 libraries to **Percussion Series** and **Platinum Bundle**:
  - **Jangdan:** focused on traditional jangdan for folk songs, rituals, pungmul
  - **Samulnori (Heritage):** more traditional setup and deeper sound than existing library
- Renamed existing Samulnori library to **Samulnori (Modern)**

---

### v1.9.1 (2024.12.23 14:42) — Added Woodwinds Polyphonic Versions + Vibrato Updates

- Added **Woodwinds Polyphonic** libraries (except Saenghwang).
  - Legato is excluded in Poly versions due to polyphonic characteristics.
- Added new controls to **Ajaeng (Jungak)**:
  - Vibrato / Portamento / Attack Time
- Improved vibrato algorithm:
  - Added **Rate** control for more realistic vibrato.

---

### v1.9.0 (2024.12.21 17:20) — LFO-Based Vibrato Update (Woodwinds + Some Strings)

- Switched vibrato from Blend to **LFO-based** control.
- Modulates **Pitch + Amplitude** for realism.
- Revised **Daepiri** keyswitch system:
  - Removed mixed Legato/Vibrato method
  - Made articulation switching more intuitive via Key Switch.
- Added LFO vibrato to woodwinds such as `Hoon`, `Jeog`, `Ji`, etc.

---

### v1.8.2 (2024.12.16 14:22) — Added Strings Polyphonic Libraries

- Added Polyphonic versions for:
  - `Ajaeng (Sanjo)`
  - `Ajaeng (Jungak)`
  - `Haegeum`
- Similar Polyphonic update planned for woodwinds.

---

### v1.8.1 (2024.11.29 16:01) — Manual & EULA Update

- Updated the manual and EULA to reflect new articulations, feature changes, and algorithm changes.

---

### v1.8.0 (2024.11.20 19:27) — Haegeum Library Update

1. Added new articulations:
   - Bendup / Bending / Tremolo  
   - Key Switch range moved one octave lower (from `C1~`) due to articulation additions.

2. Updated samples:
   - Reinforced samples from lowest range `F2` to highest range `E5` for more natural performance across a wider range.

---

### v1.7.1 (2024.11.18 14:19) — Keyswitch ↔ Articulation Dropdown Sync

- Articulation display in the top-center UI now automatically syncs when you change articulations via keyswitch.

---

### v1.7.0 (2024.11.14 15:57) — Added Legato to Monophonic Instruments

- Added Legato to monophonic woodwinds/strings (except Saenghwang) such as Daegeum, Piri family, Haegeum, Ajaeng (Jungak/Sanjo).
- Minor Taepyeongso library improvements (sound quality + bug fixes).

---

### v1.6.7 (2024.11.05 19:07) — Removed Reverb Link on CC#1 Volume + Added Saenghwang Vibrato

- Fixed an issue where reducing volume via **MIDI CC#1** also reduced/removed reverb.  
  (Volume range reset to **0 dB ~ -20 dB**)
- Added Saenghwang vibrato (nong-eum) with Depth and Rate control.

---

### v1.6.6 (2024.11.04 22:09) — Added Vibrato/Glide/Attack to Taepyeongso & Tungso + Articulation Revision

- Added real-time vibrato (CC#11), Glide Time, Attack Time.
- Revised Taepyeongso articulations and removed unnecessary ones.
  - New: Sustain (C2), Vibrato (D2), Staccato (E2), Deureum (F2), Toeseong (G2), Chuseong (A2)

---

### v1.6.5 (2024.11.02 17:32) — Added Vibrato/Glide/Attack to Sepiri & Sogeum

- Added real-time vibrato (CC#11), Glide Time, Attack Time.
- Planned rollout to other woodwinds.

---

### v1.6.4 (2024.11.01 17:25) — Range Improvements (Haegeum, Sanjo/Jungak Daegeum)

- Haegeum highest note: `C5 → Eb5`
- Daegeum (Sanjo/Jungak) highest note: `E5 → G5`

---

### v1.6.3 (2024.10.29 18:51) — Reverb Algorithm Improvement (All Libraries)

- Improved reverb tail resolution and frequency response for more natural ambience across all instruments.

---

### v1.6.2 (2024.10.28 18:15) — Added Vibrato/Glide/Attack to Piri Family + Patch Updates

- Added Glide Time and Attack Time to:
  - `Daepiri`, `Dangpiri`, `Hyangpiri`
- Daepiri:
  - Unified to Sustain; vibrato controlled via knob; intensity varies with playing strength.
- Dangpiri:
  - Added sustain behavior to all articulations except staccato.
- Hyangpiri:
  - Removed Soft Vibrato; added sustain to all articulations except staccato/chuseong/toeseong.
- Updated vibrato on other instruments (Haegeum, Sanjo Ajaeng, etc.) to be more natural.

---

### v1.6.1 (2024.10.25 15:33) — Added Vibrato/Glide/Attack to Daegeum (Sanjo/Jungak) & Danso

- Added real-time vibrato (CC#11), Glide Time, Attack Time.
- Removed `Nina` articulation due to low usage.
- Added Sustain articulation: notes sustain while holding key/pedal.

---

### v1.6.0 (2024.10.24 16:42) — Added Vibrato/Glide/Attack to Select Strings

- Updated `Haegeum` and `Ajaeng (Sanjo)`:
  - Real-time vibrato via CC#11 (Expression)
  - Glide Time (Portamento)
  - Attack Time (gradual build; default 0)
- Added MIDI note labels for articulations (Key Switch notes shown in UI).

---

### v1.5.1 (2024.10.22 20:15) — Sustain Added, GUI Update, Sample Update

- Added Sustain to all woodwinds + select strings (Sanjo Ajaeng, Jungak Ajaeng, Haegeum, etc.).
- UI now displays current articulation at the top.
- Removed unnecessary silence from fast Taepyeongso vibrato samples to improve responsiveness.
- Applied Round Robin to Samulnori janggu/kkwaenggwari for more natural repetition.

---

### v1.4.7 (2024.10.10 17:05) — Fixed Saenghwang Pitch Error + Samulnori FX Bug

- Fixed inaccurate Saenghwang pitch in certain ranges.
- Fixed an issue where FX parameters were not applied in Samulnori.

---

### v1.4.6 (2024.10.07 09:20) — Added Manual & EULA Files

- Packaged the manual and EULA in the library folder to reflect new features and license terms.

---

### v1.4.5 (2024.10.05 13:45) — Fixed Samulnori Expression Bug

- Fixed an issue where Expression did not apply correctly in some situations.

---

### v1.4.4 (2024.10.02 19:10) — Added Geomungo Articulations

- Added new Geomungo articulations such as Ssaraeng, Jachul, Chuseong, etc.

---

### v1.4.3 (2024.09.30 08:55) — Minor Bug Fix

- Fixed internal exceptions related to “Maibeo (Myber)” during parameter processing.

---

### v1.4.2 (2024.09.28 16:20) — Added Sanjo Gayageum Articulations

- Added articulations such as Chuseong, Kkeokgi + Nonghyeon, Yeonnonghyeon, Yeontwigim, Gullym, etc.

---

### v1.4.1 (2024.09.25 11:45) — Added Jungak Gayageum Articulations + 25-String Tremolo Update

- Added Jungak Gayageum “2x repeated pluck” articulation.
- Improved 25-string Gayageum tremolo sampling and expression.

---

### v1.4.0 (2024.09.22 13:30) — Added 25-String Gayageum Articulations

- Expanded articulations: 2x repeated pluck, 3x repeated pluck, Kkeokgi + Nonghyeon, Nonghyeon, Chuseong, etc.

---

### v1.3.1 (2024.09.18 21:00) — Minor Bug Fixes

- Fixed some UI display issues and setting reset problems.

---

### v1.3.0 (2024.09.15 14:10) — Major Woodwind Articulation Expansion + Daepiri Library Added

**Woodwind articulation expansion**
- Sanjo Daegeum: Nira, Noniro, Crescendo, Daruchigi
- Jungak Daegeum: Noniro, Crescendo
- Dangpiri: Nira, Nire, Noniro, Nanireu
- Sepiri: Nanireu, Nira, Nire, Nonireu
- Hyangpiri: Nanireu, Nira, Nonireu, Toeseong, Chuseong, Deep Yoseong
- Taepyeongso: fast vibrato, chuseong, toeseong, velocity layer

**Daepiri library**
- Newly added dedicated Daepiri library.

---

### v1.2.1 (2024.09.14 09:50) — Minor Bug Fixes

- Fixed issues occurring in some user environments during network updates.

---

### v1.2.0 (2024.09.12 17:20) — Minor Sample Updates + Library Additions

- Adjusted Hyangpiri and Haegeum samples to improve noise/balance issues in specific ranges.
- Added woodwind libraries: `Yak`, `Jeog`.
- Experimentally tested server-based update file delivery.

---

### v1.1.2 (2024.09.10 11:05) — Bug Fixes (Windows / iOS Partial Instrument Support)

- Improved iOS compatibility: fixed unsupported instruments in iOS environments.
- Patched Windows DS app compatibility so instruments load correctly (woodwinds, samulnori, etc.).

---

### v1.1.1 (2024.09.08 18:10) — Minor Bug Fixes

- Minor stabilization: fixed small compatibility issues and some UI display errors.

---

### v1.1.0 (2024.09.06 09:40) — Added “Ji” Library + Platinum Bundle Update

- Added standalone `Ji` library (woodwind).

---

### v1.0.1 (2024.09.04 14:25) — Minor Bug Fixes + Fixed Windows Reverb Load Error

- Fixed reverb not loading in Windows environments.
- Fixed other minor issues in some user environments.

---

### v1.0.0 (2024.09.02 10:00) — Initial Release

- Initial release of the traditional Korean instrument libraries.
