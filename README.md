<p align="center">
  <a href="#english-version"><kbd>English</kbd></a>
  <a href="#korean-version"><kbd>한국어</kbd></a>
</p>

<a id="english-version"></a>

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

### Added: Update Check File (`checkVersion.html`)

Starting from **v1.5.1**, the file `checkVersion.html` is automatically included in the folder.

- When executed, it compares your current installed version with the latest version on the server and indicates whether an update is required.
- When updating the Josun Series, you must re-download **`checkVersion.html`** together for it to work correctly.
- If the file is missing, please download `checkVersion.html` separately using the link in your original purchase email.

---

## Update History (Current Latest Version: 1.14.0)

### v1.14.0 (2026.09.22) — CC1 Dynamics & Offline Rendering Reliability Update

#### Improved CC1 Dynamics and Offline Rendering Reliability

- Improved Mod Wheel (`CC#1`) dynamics behavior across the Josun Series.
- Improved the reliability of `CC#1` automation during Cubase Offline Export and Render in Place.
- Presets now retain the same full output level as previous versions after loading, until the first `CC#1` event is received.
- Improved dynamics consistency across legato and multi-group instruments while preserving existing articulations, relative volume balance, and mixer behavior.
- Refined the `CC#1` dynamics range for smoother and more practical expressive control.

#### MIDI Channel & System Requirements

- `CC#1` Dynamics uses MIDI Channel 1.
- Minimum required Decent Sampler version: 1.19.0.

---

### v1.13.2 (2026.07.10) — Haegeum MIDI CC Control Separation Patch

#### Fixed Haegeum Vibrato / Expression MIDI Control Behavior
- Fixed an issue in the **Haegeum** library where vibrato and expression control could feel linked or behave contrary to common MIDI controller expectations.
- `CC#1` now controls expression/volume through the gain stage.
- `CC#11` now controls the Vibrato UI control, which updates only the vibrato LFO depth (`MOD_AMOUNT`).
- Adjusted the default vibrato LFO amount to prevent vibrato from being active by default when the instrument is loaded.

#### Applied Libraries
- `Haegeum (Mono)`
- `Haegeum (Poly)`

---

### v1.13.1 (2026.05.10) — Notation Software (Dorico, etc.) Playback Stability Patch & Keyswitch Structure Revamp

#### Maximized Playback Stability in Notation Software
- Completely redesigned the keyswitch routing structure to ensure 100% stable articulation transitions during playback in notation software like Dorico and Sibelius, even in environments with fast and complex MIDI data input.

#### Optimized Articulation Control Structure for All Strings & Woodwinds (30 Libraries)
- Updated from the previous indirect structure (where the sound changed via the UI menu display) to a **direct control structure**. Now, upon keyswitch input, the actual sound group changes instantly while simultaneously syncing the UI display.
- This supports flawless articulation transitions without delays or errors, even during fast passages or when stopping and restarting playback.
- **Applied to:** All 30 files across the Strings and Woodwinds libraries.

---

### v1.13.0 (2026.05.09) — Latest Decent Sampler Engine Compatibility Patch & Modulation Optimization

#### Full Compatibility & Optimization for the Latest Decent Sampler Engine
- Fully optimized the internal XML structure to align with the recently updated Decent Sampler engine. Applied compatibility patches to ensure the audio engine runs more stably and smoothly in the new player environment.

#### Vibrato Modulation Structure Enhancement
- Precisely redesigned the LFO modulation used for vibrato (Nonghyeon) at the instrument sound group level (`GROUP_TUNING`) to meet the latest engine's recommended specifications.
- This allows for smoother and more natural vibrato textures during polyphonic playing and articulation transitions.

#### Loop Point & Crossfade Precision Calibration
- Finely calibrated the sample Loop Points and Crossfade sections at the frame level for the **Haegeum**, **Daegeum (Sanjo)**, and **Jeog** libraries.
- The sustain and resonance of long notes are now much more seamless and natural.

#### Improved Percussion CC Control & Keyswitch Responsiveness
- Intuitively and efficiently optimized the `CC#1` control mapping for percussion libraries (such as **Cinematic** and **Samulnori**) and the Keyswitch On/Off routing structure for woodwinds (**Saenghwang**, **Taepyeongso**).
- Significantly improved the overall operational responsiveness of the UI controls.

---

### v1.12.2 (2026.03.28) — Convolution Reverb Equalization & Audio Capacity Optimization

- Convolution Reverb Equalization via Impulse Response Data Enhancement: Remixed the IR (Impulse Response) audio files based on loudness. This ensures a much more uniform and balanced sound when switching between different reverb types.
- Audio Capacity Optimization: Drastically reduced the file size of the instruments through a lossless audio optimization method. You can now enjoy the exact same high-quality sound with a significantly smaller storage footprint.

---

### v1.12.1 (2026.01.12) — Nabal & Nagak: Velocity Layers Added & Sound Expanded

- Nabal & Nagak Library Update: Added new audio samples to the Nabal and Nagak libraries.
- Velocity Layers Applied: Implemented velocity layers to allow sound character to change based on playing strength, resulting in a much richer and more realistic sound.

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

---

<p align="center">
  <a href="#english-version"><kbd>English</kbd></a>
  <a href="#korean-version"><kbd>한국어</kbd></a>
</p>

<a id="korean-version"></a>

# 업데이트 로그

안녕하세요, **QLAUDIO**입니다.
**조선 시리즈**의 최신 업데이트 사항을 안내드립니다.

- 새로운 업데이트 사항은 업데이트 완료 후 공지됩니다.
- 아래 최신 버전보다 오래된 버전을 사용 중이시라면, 보내드린 구매 메일 링크를 통해 재다운로드하시면 업데이트된 버전을 받으실 수 있습니다.
- 설치된 버전이 아래 최신 버전보다 이후 버전임에도 문제가 발견된다면 **contact@qlaudio.com**으로 문의해 주세요. 빠르게 확인하여 해결하겠습니다.
- 다운로드 링크에 최신 업데이트가 반영되지 않았거나 기타 문의 사항이 있으신 경우에도 같은 메일로 연락해 주세요.

감사합니다.
**QLAUDIO 드림**

---

### 업데이트 확인 파일 추가 (`checkVersion.html`)

**v1.5.1**부터 `checkVersion.html` 파일이 폴더에 자동으로 포함됩니다.

- 실행 시 현재 사용 중인 버전과 서버의 최신 버전을 비교하여 업데이트 필요 여부를 확인할 수 있습니다.
- 조선 시리즈를 업데이트하실 때는 **`checkVersion.html`**도 함께 재다운로드해야 올바르게 작동합니다.
- 파일이 없는 경우 기존 구매 메일의 다운로드 링크에서 `checkVersion.html`을 별도로 다운로드해 주세요.

---

## 업데이트 기록 (현재 최신 버전: 1.14.0)

### v1.14.0 (2026.09.22) — CC1 다이내믹 및 오프라인 렌더링 안정성 업데이트

#### CC1 다이내믹 및 오프라인 렌더링 안정성 개선

- 조선 시리즈 전반의 Mod Wheel(`CC#1`) 다이내믹 동작을 개선했습니다.
- Cubase Offline Export 및 Render in Place에서 `CC#1` 오토메이션이 더욱 안정적으로 반영되도록 개선했습니다.
- 프리셋 로드 후 첫 `CC#1` 이벤트가 입력되기 전까지 기존 버전과 동일한 최대 출력 레벨을 유지하도록 개선했습니다.
- 기존 아티큘레이션, 상대적 음량 밸런스 및 믹서 동작을 유지하면서 Legato 및 Multi-Group 악기의 다이내믹 일관성을 개선했습니다.
- 보다 자연스럽고 실용적인 강약 표현을 위해 `CC#1` 다이내믹 범위를 조정했습니다.

#### MIDI 채널 및 시스템 요구 사항

- `CC#1` 다이내믹은 MIDI Channel 1에서 동작합니다.
- 최소 요구 Decent Sampler 버전: 1.19.0

---

### v1.13.2 (2026.07.10) — 해금 MIDI CC 제어 분리 패치

#### 해금 비브라토 / 익스프레션 MIDI 제어 동작 수정
- **해금** 라이브러리에서 비브라토와 익스프레션 컨트롤이 서로 연결된 것처럼 느껴지거나, 일반적인 MIDI 컨트롤러 기대와 다르게 동작할 수 있던 문제를 수정했습니다.
- `CC#1`은 이제 gain 단계를 통해 익스프레션/볼륨을 제어합니다.
- `CC#11`은 이제 Vibrato UI control을 제어하며, 이를 통해 비브라토 LFO 깊이(`MOD_AMOUNT`)만 갱신됩니다.
- 악기 로드 직후 비브라토가 기본으로 켜진 것처럼 보이지 않도록 기본 비브라토 LFO 양을 조정했습니다.

#### 적용 라이브러리
- `Haegeum (Mono)`
- `Haegeum (Poly)`

---

### v1.13.1 (2026.05.10) — 기보 프로그램 재생 안정성 패치 및 키스위치 구조 개편

#### 기보 프로그램(Dorico 등) 재생 안정성 극대화
- Dorico, Sibelius 등 악보 제작 프로그램에서 재생 시 빠르고 복잡한 MIDI 데이터 입력 환경에서도 아티큘레이션이 안정적으로 전환되도록 키스위치 라우팅 구조를 전면 재설계했습니다.

#### 현악기 및 관악기 전체(30개 라이브러리) 아티큘레이션 제어 구조 최적화
- 기존의 UI 메뉴 표시를 거쳐 사운드가 변환되던 간접 구조에서, 키스위치 입력 시 실제 사운드 그룹이 즉시 변경되고 UI 표시도 함께 동기화되는 **직접 제어 구조**로 업데이트했습니다.
- 빠른 패시지 연주나 재생 중단 및 재시작 시에도 딜레이나 오류 없는 연주법 전환을 지원합니다.
- **적용 대상:** 현악기 및 관악기 라이브러리 전체 30개 파일

---

### v1.13.0 (2026.05.09) — 최신 Decent Sampler 엔진 호환성 패치 및 모듈레이션 최적화

#### 최신 Decent Sampler 엔진 대응 및 호환성 최적화
- 최근 업데이트된 Decent Sampler 엔진에 맞춰 내부 XML 구조를 최적화했습니다. 새로운 플레이어 환경에서도 오디오 엔진이 더 안정적이고 원활하게 동작하도록 호환성 패치를 적용했습니다.

#### 비브라토 모듈레이션 구조 고도화
- 비브라토(농현)에 사용되는 LFO 모듈레이션을 최신 엔진 권장 방식에 맞춰 악기 사운드 그룹 단위(`GROUP_TUNING`)로 재설계했습니다.
- 폴리포닉 연주 및 아티큘레이션 전환 시 더 부드럽고 자연스러운 농현 표현이 가능합니다.

#### Loop Point 및 Crossfade 정밀 보정
- **해금**, **대금(산조)**, **적** 라이브러리의 샘플 Loop Point와 Crossfade 구간을 프레임 단위로 정밀 보정했습니다.
- 롱톤 연주 시 음의 지속과 연결이 더 자연스럽게 이어집니다.

#### 타악기 CC 제어 및 Keyswitch 반응성 향상
- **Cinematic**, **Samulnori** 등 타악기 라이브러리의 `CC#1` 컨트롤 매핑과 **생황**, **태평소**의 Keyswitch On/Off 라우팅 구조를 더 직관적이고 효율적으로 최적화했습니다.
- UI 컨트롤의 전반적인 조작 반응성이 향상되었습니다.

---

### v1.12.2 (2026.03.28) — Convolution Reverb 균일화 및 음원 용량 최적화

- Impulse Response 데이터를 Loudness 기준으로 재믹싱하여 Convolution Reverb 전환 시 리버브 사운드가 더 균일하게 들리도록 개선했습니다.
- 음질 손실이 없는 방식으로 음원 용량을 최적화하여, 기존과 같은 퀄리티를 더 작은 저장 공간으로 사용할 수 있도록 했습니다.

---

### v1.12.1 (2026.01.12) — 나발 및 나각 벨로시티 레이어 추가 및 사운드 확장

- 나발과 나각 라이브러리에 새로운 음원을 추가했습니다.
- 벨로시티 레이어를 적용하여 연주 강약에 따라 소리의 성격이 달라지도록 개선했습니다.

---

### v1.12.0 (2025.12.15) — 라이브러리 통합, 악기군별 가이드 추가 및 매뉴얼 업데이트

#### RoundRobin & NoRoundRobin 라이브러리 통합
- 기존에 분리되어 있던 **RoundRobin (Default)** 라이브러리와 **NoRoundRobin** 라이브러리를 하나로 통합했습니다.
- 악기 진입 후 내부 옵션을 통해 다음 기능을 선택할 수 있습니다.
  - **RoundRobin (Default):** 연주마다 자연스러운 샘플 변화
  - **NoRoundRobin:** 고정된 샘플 재생
- **적용 라이브러리:** `Jangdan`, `Samulnori (Heritage)`, `Samulnori (Modern)`

#### Mono & Poly 라이브러리 통합
- 단선율 연주용 **Mono**와 화음 연주용 **Poly**로 나뉘어 있던 라이브러리를 하나로 통합했습니다.
- 악기 로드 후 인터페이스에서 **Mono/Poly** 모드를 직접 선택할 수 있습니다.
- **적용 라이브러리:** `Ajaeng (Jungak)`, `Ajaeng (Sanjo)`, `Haegeum`, `Danso`, `Daegeum (Jungak)`, `Daegeum (Sanjo)`,
  `Daepiri`, `Hoon`, `Jeog`, `Ji`, `Nabal`, `Nagak`, `Piri (Dang)`, `Piri (Hyang)`, `Piri (Se)`,
  `So`, `Sogeum`, `Taepyeongso`, `Tungso`, `Yak`

#### 악기군별 상세 가이드(`README.html`) 추가
- 각 폴더에 `README.html` 파일을 추가했습니다.
  - **Woodwinds**
  - **Strings**
  - **Percussion**
- 실행 시 각 악기의 연주법(**Key Switches**), **Key Mappings**, **CC controller** 기능 등을 확인할 수 있습니다.
- 기본 언어는 **영어**이며, 상단 버튼을 통해 **한국어**로 전환할 수 있습니다.

#### Manual & EULA 업데이트
- 기능 설명과 라이선스 규정(**EULA**)을 더 명확히 하기 위해 문서를 업데이트했습니다.
- **한국어 / 영어**를 지원합니다.

---

### v1.11.5 (2025.11.28) — 현악기 및 관악기 시리즈 용량 최적화

- 샘플 데이터를 최적화하여 **음질 손실 없이** 라이브러리 용량을 줄였습니다.

**용량 감소**
- 현악기 시리즈: 약 **120 MB**
- 관악기 시리즈: 약 **740 MB**

> 참고: 이번 업데이트는 기능이나 사운드 변경 없이 파일 용량만 최적화한 버전입니다.
> 기존 버전을 문제없이 사용 중이라면 필수 업데이트는 아니며, 저장 공간 확보가 필요한 경우 선택적으로 진행해 주세요.

---

### v1.11.4 (2025.11.05) — 타악기 매뉴얼 업데이트 및 Cinematic 노트 일부 수정

#### 타악기 매뉴얼 전체 검토 및 수정
- **옥타브 표기 오류 수정:** 매뉴얼 제작 시 **Concert Pitch (C1=24)**와 **컴퓨터 프로그래밍 기준 (C2=36)**이 혼용되어, Cinematic을 포함한 타악기 매뉴얼 전체가 실제보다 한 옥타브 높게 표기된 오류를 수정했습니다.
  - 예: `Chuk D7 -> D6`
- **누락 정보 추가:** **Temple & Ritual** 라이브러리의 악기 배치 정보가 누락되어 있던 문제를 수정하고 정보를 추가했습니다.

#### Cinematic 라이브러리: 일부 노트 매핑 변경
- 더 자연스러운 연주를 위해 일부 노트 범위를 변경했습니다.

- `A#4 (70) ~ D5 (74) : Yeonggo`
  → `A#4 (70) ~ D#5 (75) : Yeonggo`

- `D#5 (75) ~ F#5 (78) : Bak`
  → `E5 (76) ~ F#5 (78) : Bak`

- `A6 (93) : Nodo`
  → `A6 (93) ~ A#6 (94) : Nodo`

---

### v1.11.3 (2025.08.13) — 타악기 “Temple & Ritual” 라이브러리 추가

- **Temple & Ritual** 라이브러리를 **Percussion Series** 및 **Platinum Bundle**에 추가했습니다.
  이 라이브러리는 불교 의식과 굿 등에서 사용되는 영적이고 의식적인 타악기 사운드를 담고 있습니다.

**포함된 주요 악기**
- 법종 / 사찰 종: 작은 법종부터 웅장하고 깊은 울림의 대형 사찰 종까지 포함
- 북: 의식의 근간을 이루는 원초적이고 강력한 북소리
- 징: 장단의 시작을 알리는 깊고 넓은 울림
- 목탁: 독경 시 운율을 맞추는 맑고 명료한 소리
- 방울, 정주, 요령 등: 맑고 영적인 금속 타악기군

---

### v1.11.2 (2025.08.05) — 타악기 NoRoundRobin 버그 수정

- 일부 **NoRoundRobin** 타악기 라이브러리에서 특정 상황에 샘플이 중복 재생되던 문제를 수정했습니다.

**패치 적용 라이브러리**
- `Jangdan (NoRoundRobins)`
- `Samulnori (Heritage) (NoRoundRobins)`
- `Samulnori (Modern) (NoRoundRobins)`

---

### v1.11.1 (2025.07.02) — 나발 및 나각 추가

- **나발**과 **나각** 라이브러리를 **Woodwinds Series**에 추가했습니다.
- 두 악기 모두 실제로는 단일 음정을 내는 악기지만, 사용 편의성을 위해 한 옥타브 내 모든 음정을 연주할 수 있도록 구현했습니다.

**나발**
- 긴 금속관으로 만들어진 관악기로 깊고 우렁찬 단일음을 냅니다.
- 지공이 없어 멜로디 연주보다는 대취타 등에서 장엄한 분위기 연출이나 신호용으로 사용됩니다.

**나각**
- 커다란 소라 껍데기로 만든 자연 악기입니다.
- 뱃고동처럼 깊고 웅장한 소리를 내며, 대취타 등에서 신비롭고 장엄한 분위기를 더합니다.

---

### v1.11.0 (2025.06.04) — 전체 관악기 및 현악기 Keyswitch On/Off 기능 추가

- UI에 **Keyswitch** 버튼을 추가했습니다.
- 건반을 통한 아티큘레이션 변경(**Keyswitch**) 기능을 실시간으로 켜고 끌 수 있습니다.

**동작 방식**
- **Keyswitch ON (기본값):**
  - 기존과 동일하게 특정 건반으로 아티큘레이션을 변경합니다.
  - 키스위치 건반은 UI 가상 건반에 시각적으로 표시됩니다.
- **Keyswitch OFF:**
  - 키스위치로 지정된 건반이 일반 연주용 건반처럼 동작하거나, 샘플이 없는 경우 아무 동작도 하지 않습니다.
  - 아티큘레이션 변경은 UI 드롭다운 메뉴로만 가능합니다.
  - 키스위치 색상 표시가 사라집니다.

**적용 대상**
- **현악기:** 가야금(정악, 산조, 25현), 거문고(정악, 산조), 아쟁(정악, 산조), 해금
- **관악기:** 대금(정악, 산조), 소금, 중금, 단소, 퉁소, 생황, 태평소, 향피리, 세피리, 당피리, 대피리, 지, 약, 적, 훈 등 기존 Keyswitch 기능이 있던 모든 관악기

**사용자 편의성**
- 복잡한 시퀀싱 작업 중 의도치 않은 키스위치 입력을 방지하거나, 특정 상황에서 키스위치 영역을 연주용으로 활용할 수 있습니다.

**UI / 안정성**
- Keyswitch On/Off 버튼 추가에 따라 일부 UI 배치 및 가독성을 개선했습니다.
- 내부 스크립트 최적화를 통해 Keyswitch 기능의 안정성과 반응성을 향상했습니다.

---

### v1.10.0 (2025.04.30) — Convolution Reverb 타입 선택 기능 및 매뉴얼 업데이트

#### IR 타입 선택 드롭다운 추가
- 옵션:
  `cathedral.wav` / `chamber.wav` / `dream.wav` / `hall.wav` / `large_hall.wav` / `outdoor.wav` / `plate.wav` / `room.wav` / `studio.wav`
- 기본값: `hall.wav`

#### Reverb 타입별 설명
- **Cathedral:** 거대한 공간감과 풍부한 저역으로 웅장하고 신비로운 분위기를 연출합니다.
- **Chamber:** 부드럽고 따뜻한 울림으로 친밀하고 자연스러운 실내감을 제공합니다.
- **Dream:** 은은한 잔향으로 몽환적이고 에테리얼한 느낌을 강조합니다.
- **Hall:** 균형 잡힌 반사음으로 자연스러운 공간감을 유지합니다.
- **Large Hall:** 넓고 풍부한 반사음으로 웅장한 무대감을 제공합니다.
- **Outdoor:** 야외 공간처럼 탁 트인 느낌을 제공합니다.
- **Plate:** 밝고 선명한 반사음으로 반짝이는 울림을 강조합니다.
- **Room:** 아늑하고 현실적인 실내 반사음을 제공합니다.
- **Studio:** 깔끔함을 해치지 않는 은은한 깊이감을 더합니다.

#### 매뉴얼 업데이트
- IR 타입 선택 기능 설명을 추가했습니다.
- 타악기 RoundRobin / NoRoundRobin 설명을 보강했습니다.
- 기타 오타 및 표현을 개선했습니다.

---

### v1.9.9 (2025.04.08 09:24) — 타악기 NoRoundRobin 라이브러리 추가

- 다음 라이브러리에 **NoRoundRobin** 버전을 추가했습니다.
  - `Jangdan`
  - `Samulnori (Heritage)`
  - `Samulnori (Modern)`

**Round Robin**
- 타악기 연주의 자연스러움을 위해 연주할 때마다 다른 샘플 베리에이션을 재생하는 기능입니다.

**장점**
- 같은 노트를 반복해도 서로 다른 샘플이 재생되어 인위적인 반복감을 줄일 수 있습니다.

**단점**
- 항상 동일한 샘플 재생이 필요한 경우에는 불필요할 수 있습니다.

- 사용자 선택 폭을 넓히기 위해 NoRoundRobin 라이브러리를 추가했습니다.

---

### v1.9.8 (2025.04.02 12:58) — 장단 변죽 삼연음 샘플 리소스 수정

- 장단 라이브러리의 변죽 삼연음 샘플 앞부분에 공백이 있어 재생이 밀리던 문제를 수정했습니다.

---

### v1.9.7 (2025.03.14 14:50) — 전체 라이브러리 Convolution Reverb 기본 믹스 최적화

- Convolution Reverb 기본 믹스 값을 변경했습니다.
  - **0.30 (30%) → 0.15 (15%)**
- 기존 기본값의 리버브가 과도하다는 피드백을 반영하여 테스트 후 최적화했습니다.

---

### v1.9.6 (2025.03.02 13:12) — 사물놀이 악기별 볼륨 및 패닝 노브 추가

- `Samulnori (Modern)` 및 `Samulnori (Heritage)` 라이브러리를 업데이트했습니다.
- 장구, 꽹과리 등 각 악기별 **Volume** 및 **Panning** 노브를 추가하여 더 정밀한 믹싱과 사운드 디자인이 가능해졌습니다.

---

### v1.9.5 (2025.02.19 14:41) — 딜레이 타임 노브 추가 및 거문고 산조(Poly) 보이스 오류 수정

#### 딜레이 타임 컨트롤 노브 추가
- 딜레이 타임을 직접 조절할 수 있는 노브를 추가했습니다.
- **Time Sync:** DAW BPM에 자동으로 연동됩니다.
- **Musical values:** 16분음표, 4분음표 등 음악적 단위로 선택할 수 있습니다.
- **실시간 반영:** 노브 조작 시 즉시 반영되어 직관적인 사운드 디자인이 가능합니다.

#### 거문고 산조(Poly) 보이스 오류 수정
- Basic 연주법에서 Vibrato 음이 동시에 나는 문제를 수정했습니다.

---

### v1.9.4 (2025.01.22 13:05) — Portamento Glide Time 수정

- Portamento 동작을 개선했습니다.
  - 더 자연스러운 음 간 연결 시간 조절
  - 중간 구간의 섬세한 조절 및 후반 구간의 큰 변화
  - 반응 곡선 최적화
  - 이전 버전의 급격하거나 예상치 못한 동작 수정

---

### v1.9.3 (2025.01.06 15:23) — 장단 및 사물놀이(Heritage) 추가, 사물놀이 명칭 변경

- **Percussion Series** 및 **Platinum Bundle**에 2개 라이브러리를 추가했습니다.
  - **Jangdan:** 민요, 의식, 풍물 등 전통 장단 연주에 특화된 라이브러리
  - **Samulnori (Heritage):** 기존 라이브러리보다 더 전통적인 구성과 깊이 있는 사운드
- 기존 사물놀이 라이브러리 명칭을 **Samulnori (Modern)**으로 변경했습니다.

---

### v1.9.1 (2024.12.23 14:42) — 관악기 Polyphonic 버전 추가 및 비브라토 업데이트

- **Saenghwang**을 제외한 관악기 Polyphonic 라이브러리를 추가했습니다.
  - Polyphonic 특성상 Mono 버전의 Legato 기능은 제외되었습니다.
- **Ajaeng (Jungak)**에 신규 컨트롤을 추가했습니다.
  - Vibrato / Portamento / Attack Time
- 비브라토 알고리즘을 개선했습니다.
  - **Rate** 컨트롤을 추가하여 더 현실적인 비브라토 표현이 가능합니다.

---

### v1.9.0 (2024.12.21 17:20) — LFO 기반 비브라토 업데이트

- 기존 Blend 방식에서 **LFO 기반** 비브라토 컨트롤로 전환했습니다.
- **Pitch + Amplitude**를 함께 모듈레이션하여 더 사실적인 비브라토를 구현했습니다.
- **Daepiri** 키스위치 방식을 수정했습니다.
  - Legato와 Vibrato가 섞여 있던 방식을 제거했습니다.
  - Key Switch로 연주법을 더 직관적으로 전환하도록 개선했습니다.
- `Hoon`, `Jeog`, `Ji` 등 여러 관악기에 LFO 기반 비브라토를 추가했습니다.

---

### v1.8.2 (2024.12.16 14:22) — 현악기 Polyphonic 라이브러리 추가

- 다음 라이브러리의 Polyphonic 버전을 추가했습니다.
  - `Ajaeng (Sanjo)`
  - `Ajaeng (Jungak)`
  - `Haegeum`
- 관악기에도 동일한 형태의 Polyphonic 업데이트가 적용될 예정입니다.

---

### v1.8.1 (2024.11.29 16:01) — Manual & EULA 업데이트

- 최근 버전의 신규 연주법, 기능 변경, 알고리즘 변경사항을 Manual 및 EULA에 반영했습니다.

---

### v1.8.0 (2024.11.20 19:27) — 해금 라이브러리 업데이트

1. 새로운 연주법을 추가했습니다.
   - Bendup / Bending / Tremolo
   - 연주법 추가에 따라 Key Switch 범위가 한 옥타브 아래(`C1~`)로 이동했습니다.

2. 음원을 업데이트했습니다.
   - 가장 낮은 음역 `F2`부터 가장 높은 음역 `E5`까지 음원을 보강하여 더 넓은 음역대에서 자연스러운 연주가 가능합니다.

---

### v1.7.1 (2024.11.18 14:19) — Keyswitch와 Articulation Dropdown UI 동기화

- 키스위치로 연주법을 변경하면 중앙 상단 UI의 Articulation 표시가 자동으로 동기화되도록 개선했습니다.

---

### v1.7.0 (2024.11.14 15:57) — 모노포닉 악기 Legato 기능 추가

- 생황을 제외한 대금, 피리류, 해금, 아쟁(정악/산조) 등 모노포닉 관악기 및 현악기에 Legato 기능을 추가했습니다.
- 태평소 라이브러리의 음질 개선 및 버그 수정을 진행했습니다.

---

### v1.6.7 (2024.11.05 19:07) — CC#1 볼륨 조절 시 리버브 연동 제거 및 생황 비브라토 추가

- **MIDI CC#1**로 볼륨을 줄일 때 리버브가 함께 줄거나 사라지던 문제를 수정했습니다.
  (볼륨 범위 **0 dB ~ -20 dB**로 재설정)
- 생황 라이브러리에 비브라토(농음) 기능을 추가하고 Depth / Rate 컨트롤을 지원했습니다.

---

### v1.6.6 (2024.11.04 22:09) — 태평소 및 퉁소 비브라토/글라이드/어택 추가, 연주법 수정

- 실시간 비브라토(CC#11), Glide Time, Attack Time 기능을 추가했습니다.
- 태평소 연주법을 수정하고 불필요한 연주법을 제거했습니다.
  - 변경 후: Sustain (C2), Vibrato (D2), Staccato (E2), Deureum (F2), Toeseong (G2), Chuseong (A2)

---

### v1.6.5 (2024.11.02 17:32) — 세피리 및 소금 비브라토/글라이드/어택 추가

- 실시간 비브라토(CC#11), Glide Time, Attack Time 기능을 추가했습니다.
- 다른 관악기에도 순차 적용 예정입니다.

---

### v1.6.4 (2024.11.01 17:25) — 일부 라이브러리 음역대 개선

- 해금 최고음역: `C5 → Eb5`
- 대금(산조/정악) 최고음역: `E5 → G5`

---

### v1.6.3 (2024.10.29 18:51) — 전체 라이브러리 리버브 알고리즘 개선

- 잔향 해상도 및 주파수 반응을 개선하여 전체 악기에서 더 자연스러운 공간감을 구현했습니다.

---

### v1.6.2 (2024.10.28 18:15) — 피리 계열 비브라토/글라이드/어택 추가 및 패치

- 다음 악기에 Glide Time 및 Attack Time을 추가했습니다.
  - `Daepiri`, `Dangpiri`, `Hyangpiri`
- Daepiri:
  - Sustain 단일 연주법으로 통합하고, 비브라토는 노브로 제어하도록 변경했습니다.
  - 연주 강세에 따라 비브라토 강도가 달라집니다.
- Dangpiri:
  - 스타카토를 제외한 모든 연주법에 Sustain 동작을 추가했습니다.
- Hyangpiri:
  - Soft Vibrato를 제거했습니다.
  - 스타카토, 추성, 퇴성을 제외한 모든 연주법에 Sustain 동작을 추가했습니다.
- 해금, 산조 아쟁 등 다른 악기의 비브라토도 더 자연스럽게 업데이트했습니다.

---

### v1.6.1 (2024.10.25 15:33) — 대금(산조/정악) 및 단소 비브라토/글라이드/어택 추가

- 실시간 비브라토(CC#11), Glide Time, Attack Time 기능을 추가했습니다.
- 활용 빈도가 낮은 `Nina` 연주법을 제거했습니다.
- 건반이나 페달을 누르고 있는 동안 음이 유지되는 Sustain 연주법을 추가했습니다.

---

### v1.6.0 (2024.10.24 16:42) — 일부 현악기 비브라토/글라이드/어택 추가

- `Haegeum` 및 `Ajaeng (Sanjo)`를 업데이트했습니다.
  - CC#11(Expression)을 통한 실시간 비브라토
  - Glide Time(Portamento)
  - Attack Time(서서히 커지는 음정 효과, 기본값 0)
- Key Switch 노트를 UI에 표시하여 연주법을 쉽게 확인할 수 있도록 했습니다.

---

### v1.5.1 (2024.10.22 20:15) — Sustain 기능 추가, GUI 업데이트, 음원 업데이트

- 모든 관악기 및 일부 현악기(산조 아쟁, 정악 아쟁, 해금 등)에 Sustain 기능을 추가했습니다.
- UI 상단에 현재 연주법을 표시하도록 개선했습니다.
- 태평소 빠른 농음 샘플 시작부의 불필요한 공백을 제거해 반응성을 높였습니다.
- 사물놀이 장구/꽹과리에 Round Robin을 적용하여 반복 재생 시 더 자연스럽게 들리도록 했습니다.

---

### v1.4.7 (2024.10.10 17:05) — 생황 음정 오류 및 사물놀이 FX 버그 수정

- 특정 음역대에서 생황 음정이 부정확하게 나는 문제를 수정했습니다.
- 사물놀이 라이브러리에서 FX 파라미터가 적용되지 않던 문제를 수정했습니다.

---

### v1.4.6 (2024.10.07 09:20) — Manual & EULA 파일 추가

- 버전 업데이트 후 추가된 연주법과 라이선스 내용을 반영한 Manual 및 EULA 파일을 라이브러리 폴더에 포함했습니다.

---

### v1.4.5 (2024.10.05 13:45) — 사물놀이 Expression 버그 수정

- 일부 상황에서 Expression이 정상 반영되지 않던 문제를 수정했습니다.

---

### v1.4.4 (2024.10.02 19:10) — 거문고 연주법 추가

- 싸랭, 자출, 추성 등 새로운 거문고 연주법을 추가했습니다.

---

### v1.4.3 (2024.09.30 08:55) — 마이너 버그 수정

- 내부 파라미터 처리 과정에서 발생하던 “마이버(Myber)” 관련 예외를 수정했습니다.

---

### v1.4.2 (2024.09.28 16:20) — 산조 가야금 연주법 추가

- 추성, 꺾기+농현, 연농현, 연튀김, 굴림 등 산조 가야금 연주법을 추가했습니다.

---

### v1.4.1 (2024.09.25 11:45) — 정악 가야금 연주법 추가 및 25현 가야금 트레몰로 보강

- 정악 가야금 2회연튕김 연주법을 추가했습니다.
- 25현 가야금 트레몰로 샘플링과 표현력을 개선했습니다.

---

### v1.4.0 (2024.09.22 13:30) — 25현 가야금 연주법 추가

- 2회연튕김, 3회연튕김, 꺾기+농현, 농현, 추성 등 25현 가야금 연주법을 확장했습니다.

---

### v1.3.1 (2024.09.18 21:00) — 마이너 버그 수정

- 일부 UI 표시 오류와 설정값 리셋 문제를 수정했습니다.

---

### v1.3.0 (2024.09.15 14:10) — 관악기 연주법 대폭 확장 및 대피리 라이브러리 추가

**관악기 연주법 확장**
- 산조대금: Nira, Noniro, Crescendo, Daruchigi
- 정악대금: Noniro, Crescendo
- 당피리: Nira, Nire, Noniro, Nanireu
- 세피리: Nanireu, Nira, Nire, Nonireu
- 향피리: Nanireu, Nira, Nonireu, Toeseong, Chuseong, Deep Yoseong
- 태평소: 빠른농음, Chuseong, Toeseong, Velocity Layer

**대피리 라이브러리**
- 전용 대피리 라이브러리를 새롭게 추가했습니다.

---

### v1.2.1 (2024.09.14 09:50) — 마이너 버그 수정

- 네트워크 업데이트 시 일부 사용자 환경에서 발생하던 문제를 수정했습니다.

---

### v1.2.0 (2024.09.12 17:20) — 마이너 음원 업데이트 및 라이브러리 추가

- 향피리와 해금 샘플의 특정 음역대 노이즈 및 밸런스 문제를 개선했습니다.
- 관악기 라이브러리 `Yak`, `Jeog`를 추가했습니다.
- 서버 기반 업데이트 파일 전송 방식을 실험적으로 테스트했습니다.

---

### v1.1.2 (2024.09.10 11:05) — Windows / iOS 일부 악기 미지원 오류 수정

- iOS 환경에서 특정 악기가 지원되지 않던 문제를 수정했습니다.
- Windows DS 앱에서 관악기, 사물놀이 등 악기가 정상 로드되도록 호환성 패치를 적용했습니다.

---

### v1.1.1 (2024.09.08 18:10) — 마이너 버그 수정

- 일부 호환성 문제와 UI 표시 오류를 수정했습니다.

---

### v1.1.0 (2024.09.06 09:40) — 지 라이브러리 및 플래티넘 번들 업데이트

- 관악기 `Ji` 라이브러리를 별도 악기로 추가했습니다.

---

### v1.0.1 (2024.09.04 14:25) — 마이너 버그 수정 및 Windows 리버브 로드 오류 수정

- Windows 환경에서 리버브가 로드되지 않던 문제를 수정했습니다.
- 일부 사용자 환경에서 발생하던 경미한 오류를 수정했습니다.

---

### v1.0.0 (2024.09.02 10:00) — 초기 릴리스

- 국악기 라이브러리의 초기 기능을 포함한 최초 버전입니다.
