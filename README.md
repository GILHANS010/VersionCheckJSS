Update Log

Hello, this is QLAUDIO.
We would like to inform you of the update details for the Josun Series.

New update information will be announced after the update is completed.

After checking the update history below, if you are using a version prior to the latest update, you can re-download the product via the purchase email link we sent you to receive the newly updated version.

If you discover an issue even though your installed version is already newer than the one listed (i.e., installed after the relevant update), please do not hesitate to contact us at contact@qlaudio.com
 and we will resolve it promptly.

If the download link does not reflect the latest update, or if you have any other inquiries, please contact us at the same email address and we will assist you as quickly as possible.

Thank you.
Sincerely,
QLAUDIO

<Added Update Check File>

The file checkVersion.html will be automatically added to the folder starting from version 1.5.1.
When executed, it compares your current version with the latest version on the server and lets you know whether an update is required.

When updating the Josun Series, you must re-download checkVersion.html together for it to work correctly.
If you do not have the file, please download checkVersion.html separately via the link in your original purchase email.

<Update History> (Current Latest Version = 1.12.0)
Version 1.12.0 (2025.12.15) — Library integration, per-instrument-group guides added, and manual updated

RoundRobin & NoRoundRobin library integration:
The previously separated RoundRobin (default) library and NoRoundRobin library have been merged into one. After entering an instrument, you can now choose between RoundRobin (Default), which naturally varies the sound, and NoRoundRobin, which uses fixed samples, via internal options.
Applied libraries: Jangdan, Samulnori (Heritage), Samulnori (Modern)

Mono & Poly library integration:
The libraries that were previously split into Monophonic (Mono) for single-note performance and Polyphonic (Poly) for chord performance have been merged into one. After loading an instrument, you can directly select Mono/Poly mode within the interface and perform accordingly.
Applied libraries: Ajaeng (Jungak), Ajaeng (Sanjo), Haegeum, Danso, Daegeum (Jungak), Daegeum (Sanjo), Daepiri, Hoon, Jeog, Ji, Nabal, Nagak, Piri (Dang), Piri (Hyang), Piri (Se), So, Sogeum, Taepyeongso, Tungso, Yak

Added detailed per-instrument-group guide (README) files:
A README.html file containing detailed information for each instrument has been added inside each folder for Woodwinds, Strings, and Percussion.
By running the file, you can review each instrument’s playing methods (Key Switches), key mappings, CC controller functions, and more in detail.
The default language is English, and you can also view the contents in Korean via the button at the top.

Updated the integrated manual and EULA files:
Documents have been updated to provide clearer feature explanations and to explicitly state the license terms (EULA). (Korean/English supported)

Version 1.11.5 (2025.11.28) — Storage optimization for Strings and Woodwinds series

Library size optimization: Reduced library size without audio quality loss by optimizing sample data.

Strings series: approx. 120MB reduced
Woodwinds series: approx. 740MB reduced

(Reference) This update only optimizes file size without any functional or sound changes. Therefore, if you are using the existing version without issues, updating is not mandatory. Please update only if you need to free up storage space.

Version 1.11.4 (2025.11.05) — Percussion series manual update and partial note fixes in the Cinematic library

Reviewed and revised the entire Percussion series manual.

Fixed octave notation error:
During manual creation, a mix-up between “Concert Pitch (C1=24)” and “Computer programming standard (C2=36)” caused the entire percussion manual—including the Cinematic library—to be notated one octave higher than the actual instruments. This has been corrected. (Example: “Chuk” D7 → D6)

Added missing information:
Fixed an issue where instrument placement information for the “Temple & Ritual” library was missing from the manual, and added the information.

Partial note fixes in the Cinematic library

Cinematic note mapping changes: Some notes were changed for more natural performance.
A#4 (70) ~ D5 (74): Yeonggo → A#4 (70) ~ D#5 (75): Yeonggo
D#5 (75) ~ F#5 (78): Bak → E5 (76) ~ F#5 (78): Bak
A6 (93): Nodo → A6 (93) ~ A#6 (94): Nodo

Version 1.11.3 (2025.8.13) — Added “Temple & Ritual” library to the Percussion series

A new “Temple & Ritual” library has been added to the Percussion series and the Platinum Bundle. This library contains spiritual and ritual percussion sounds used in Buddhist ceremonies and shamanistic rituals (gut).

Main included instruments:

Buddhist bell / temple bell: From small ritual bells to large temple bells with grand, deep resonance

Drum: Primitive and powerful drum sounds like a heartbeat that form the foundation of rituals

Jing (large gong): A deep and wide resonance that signals the start of jangdan in gut or pungmul

Moktak (wooden fish): Clear and articulate moktak sounds used to keep rhythm during chanting

Hand bells, Jeongju, Yoryeong, etc.: Various clear and spiritual metal percussion instruments used for purification

Version 1.11.2 (2025.8.5)

Fixed an error in Percussion NoRoundRobin libraries
A bug was fixed where samples could play duplicated in some situations in certain percussion libraries without Round Robin.
Patched libraries: Jangdan (NoRoundRobins), Samulnori (Heritage) (NoRoundRobins), Samulnori (Modern) (NoRoundRobins)

Version 1.11.1 (2025.7.2)

Added Nabal and Nagak libraries to the Woodwinds series and the Platinum Bundle
New Nabal and Nagak instrument libraries have been added to the Woodwinds series.
Although both instruments can produce only a single pitch in reality, for usability we enabled them to play all notes within one octave.

Nabal: A brass instrument made from long metal, producing a deep, resonant single tone like a trombone. It has no finger holes and cannot play melodies; it is used in daechwita (military ceremonial music) to create a solemn atmosphere or to send signals.

Nagak: A natural instrument made from a large conch shell, characterized by a deep and majestic sound like a foghorn. It produces a single sustained tone without melody and adds a mysterious and solemn atmosphere in daechwita and similar contexts.

Version 1.11.0 (2025.6.4)

Added Keyswitch On/Off feature to all Woodwinds and Strings libraries
A new “Keyswitch” button has been added to the user interface (UI).
Using this button, you can toggle each instrument’s keyboard-based articulation switching (Keyswitch) function on and off in real time.

Function details:

Keyswitch ON (default): Same as before—you can change articulations by pressing specific keys, and those keyswitch keys are also visually indicated on the UI’s virtual keyboard.

Keyswitch OFF: The keys assigned as keyswitches will either behave like normal playable keys (if samples are mapped to that range) or do nothing. Articulation changes will only be possible through the UI dropdown menu. In this state, the special color indication for keyswitch keys also disappears.

Applied libraries:

Strings: Gayageum (Jungak, Sanjo, 25-string), Geomungo (Jungak, Sanjo), Ajaeng (Jungak, Sanjo), Haegeum

Woodwinds: Daegeum (Jungak, Sanjo), Sogeum, Junggeum, Danso, Tungso, Saenghwang, Taepyeongso, Hyangpiri, Sepiri, Dangpiri, Daepiri, Ji, Yak, Jeog, Hoon, etc. (all woodwinds that previously had keyswitch functionality)

Improved usability: Useful for preventing unintended keyswitch inputs during complex sequencing, or for using the keyswitch range as playable keys in certain situations.

UI improvements:
Minor improvements to control layout and readability (where applicable) following the addition of the Keyswitch On/Off button.

Other:
Improved stability and responsiveness of the Keyswitch function via internal script optimization.

Version 1.10.0 (2025.4.30)

Added Convolution Reverb type selection feature

Added dropdown menu to select IR files

Options: cathedral.wav / chamber.wav / dream.wav / hall.wav / large_hall.wav / outdoor.wav / plate.wav / room.wav / studio.wav

Default: hall.wav

Descriptions by reverb type:

Cathedral: Adds a vast sense of space with rich low-end resonance, creating a grand and mysterious atmosphere.

Chamber: Soft and warm resonance that preserves an intimate yet natural indoor character.

Dream: Subtle, translucent reverb tails that emphasize a dreamy, ethereal feel.

Hall: Balanced reflections that spread cleanly, maintaining a natural sense of space.

Large Hall: Provides a wide, lush reflection stage for a grand, stage-like feeling.

Outdoor: Simulates open-air space with gently diffusing reflections for a fresh, open feel.

Plate: Bright, shimmering reflections that emphasize a clear and crisp resonance.

Room: Expresses cozy, realistic early reflections to add natural intimacy.

Studio: Provides only subtle studio reflections, adding nuanced depth without compromising clarity.

Manual update:

Added explanation of the reverb type selection feature

Expanded explanations for Percussion Round Robin and NoRoundRobin libraries

Other typo and wording improvements

Version 1.9.9 (2025.4.8 09:24) — Added percussion libraries with Round Robin removed

Added NoRoundRobin libraries (Round Robin removed) for Jangdan, Samulnori (Heritage), and Samulnori (Modern).

Round Robin: A feature that plays different sample variations each time you perform, to make percussion performance sound more natural.

Pros: Reduces artificial repetition by triggering different samples even when playing the same note.

Cons: If you want the exact same sample every time, it can be unnecessary.

By adding NoRoundRobin libraries, we provide users with broader choices.

Version 1.9.8 (2025.4.2 12:58) — Fixed resource for “byeonjuk triplet” samples in the Jangdan library

Fixed an issue where silence at the beginning of the byeonjuk triplet sample in the Jangdan library caused the sound to be delayed.

Version 1.9.7 (2025.3.14 14:50) — Optimized Convolution Reverb mix parameter value across all libraries

Updated the default Convolution Reverb mix parameter value across all libraries:
Default Mix Value: 0.3 (30%) → 0.15 (15%)
→ Based on feedback that the previous default mix was too strong, we tested and changed it to the most optimized value.

Version 1.9.6 (2025.3.2 13:12) — Added per-instrument volume and panning control knobs to Samulnori libraries

Updated Samulnori (Modern and Heritage) libraries

Added volume and panning control knobs for each instrument
→ Users can now adjust volume and left-right panning individually for each instrument (e.g., janggu, kkwaenggwari), enabling more precise mixing and sound design.

Version 1.9.5 (2025.2.19 14:41) — Added delay time knob and fixed Geomungo Sanjo (Poly) voice error

Added delay time control knob

Added a new delay time knob so users can directly control delay time.

Time Sync: Implements Time Sync that automatically follows the DAW’s BPM, adjusting delay time according to tempo changes.

Fine adjustment: Can be set in musical time units (e.g., 16th note, quarter note) for more intuitive control.

Real-time response: Immediately reflected when operating the knob for intuitive sound design.

Fixed Geomungo Sanjo (Poly) voice error

Resolved an issue where vibrato notes would sound simultaneously during Basic articulation in the Sanjo Geomungo library.

Version 1.9.4 (2025.1.22 13:05) — Portamento Glide Time revision

Portamento parameter improvements

Smoother connection time control: Improved to allow more natural control of connection time between notes via the knob.

More delicate control: Improved so the mid-range allows fine adjustment, while the latter range produces larger changes.

Curve adjustment: Optimized the Portamento effect curve by changing internal settings.

Issue resolved: Fixed problems in previous versions where the Portamento effect changed too abruptly or produced unexpected results.

Version 1.9.3 (2025.1.06 15:23) — Added Jangdan and Samulnori (Heritage) libraries

Added two new libraries to the Percussion Series and Platinum Bundle:

Jangdan library: A percussion library specialized for traditional jangdan performance frequently used in folk songs, rituals, and pungmul.

Samulnori (Heritage) library: Compared to the existing Samulnori library, it delivers a more traditional instrument configuration and deeper sound.

Samulnori library name change

The existing Samulnori library has been renamed to Samulnori (Modern).

Version 1.9.1 (2024.12.23 14:42) — Added Woodwinds Polyphonic Library, added vibrato, and updated vibrato algorithm

Added Woodwinds Series polyphonic library (except Saenghwang)

Added polyphonic versions for woodwinds that were previously monophonic only.

Due to polyphonic characteristics, the Legato function used in monophonic versions is not included.

Added Vibrato, Portamento, Attack Time controls to Ajaeng (Jungak)

Introduced new controls (Vibrato, Portamento, Attack Time) to improve expressiveness.

Improved vibrato algorithm

Added Rate control as well, enabling vibrato expression closer to real instruments.

Version 1.9.0 (2024.12.21 17:20) — Updated vibrato algorithm for all Woodwinds and some Strings libraries

Updated vibrato algorithm to an LFO-based approach

Switched from the previous Blend method to LFO-based vibrato control.

Modulates both Pitch and Amplitude to implement more realistic vibrato.

Changed Daepiri keyswitch method

Removed the previous approach where Legato and Vibrato were mixed, and revised it so playing methods can be switched more intuitively via Key Switch.

Added vibrato to other Woodwinds libraries

Added LFO-based vibrato to multiple woodwinds such as Hoon, Jeog, Ji, etc., which previously had no vibrato.

Version 1.8.2 (2024.12.16 14:22) — Added Strings Series polyphonic libraries

Added polyphonic versions for three Strings Series libraries: Sanjo Ajaeng, Jungak Ajaeng, and Haegeum.

The same type of Polyphonic update is planned to be applied to woodwinds libraries soon.

Version 1.8.1 (2024.11.29 16:01) — Updated user manual and EULA

Updated the manual and EULA to reflect newly added playing methods, feature changes, and algorithm changes in recent versions.

Version 1.8.0 (2024.11.20 19:27) — Haegeum library update

Added Bendup, Bending, and Tremolo playing methods to the Haegeum library

As new playing methods were added, the Key Switch range was moved one octave lower (from C1~).

Updated Haegeum samples

Enhanced samples from the lowest range (F2) to the highest range (E5), enabling more natural performance over a wider range.

Version 1.7.1 (2024.11.18 14:19) — Keyswitch & Articulation UI synchronization

When changing articulations via keyswitch, the playing method display at the top center of the UI is now automatically synchronized.

Version 1.7.0 (2024.11.14 15:57) — Added Legato to monophonic instruments

Added Legato to monophonic instruments (except Saenghwang) such as Daegeum, Piri family, Haegeum, and Ajaeng (Jungak/Sanjo) so notes connect naturally during fast passages.

Taepyeongso library sample improvement

Performed a minor update related to sound quality improvements and bug fixes.

Version 1.6.7 (2024.11.05 19:07) — Removed reverb-level linkage when controlling volume via MIDI CC#1, and added Saenghwang vibrato control

Resolved reverb level linkage issue

Fixed an issue where reducing volume via MIDI CC#1 would also reduce/remove reverb. (Volume range reset to 0dB ~ -20dB)

Added Saenghwang vibrato control

Added vibrato (nong-eum) to the Saenghwang library with detailed control via Depth and Rate.

Version 1.6.6 (2024.11.04 22:09) — Added vibrato, portamento (glide), attack time to Taepyeongso and Tungso; revised playing methods

Added vibrato (nonghyeon), portamento, and attack time features

Added real-time vibrato (MIDI CC#11), Glide Time, and Attack Time controls to Taepyeongso and Tungso libraries.

Revised Taepyeongso playing methods

Added a knob to control the timing of vibrato in real time, and removed previously unnecessary playing methods.

New playing methods: Sustain (C2), Vibrato (D2), Staccato (E2), Deureum (F2), Toeseong (G2), Chuseong (A2)

Version 1.6.5 (2024.11.02 17:32) — Added vibrato, portamento (glide), attack time to Sepiri and Sogeum

Added vibrato, portamento, and attack time controls

Added real-time vibrato (MIDI CC#11), Glide Time, and Attack Time controls to Sepiri and Sogeum libraries.

Planned rollout to other woodwinds

The same functions will be applied sequentially to other woodwinds libraries as well.

Version 1.6.4 (2024.11.01 17:25) — Improved ranges for certain libraries (Haegeum, Sanjo Daegeum, Jungak Daegeum)

Haegeum range expansion: Highest note improved from C5 → Eb5

Daegeum (Sanjo/Jungak) range expansion: Highest note improved from E5 → G5

Version 1.6.3 (2024.10.29 18:51) — Reverb algorithm improvement (all instrument libraries)

Adjusted the reverb algorithm to improve tail resolution and frequency response, delivering more natural reverb across all instruments.

Version 1.6.2 (2024.10.28 18:15) — Added vibrato, portamento, attack time to Daepiri/Dangpiri/Hyangpiri; revised patches

Added vibrato (MIDI CC#11), portamento, and attack time

Added Glide Time and Attack Time controls to Daepiri, Dangpiri, and Hyangpiri for richer expression.

Daepiri patch

Unified into a single Sustain articulation, and changed to control vibrato via a Vibrato knob.

Vibrato intensity varies depending on playing strength.

Dangpiri patch

Added “sustain” behavior to all articulations except staccato, so notes are held during performance.

Hyangpiri patch

Removed Soft Vibrato, which had minimal effect.

Added “sustain” behavior to all articulations except staccato, chuseong, and toeseong.

Improved vibrato algorithm

Updated vibrato on other instruments (e.g., Haegeum, Sanjo Ajaeng) to be more natural.

Version 1.6.1 (2024.10.25 15:33) — Added vibrato, portamento, attack time to Daegeum (Sanjo/Jungak) and Danso

Added vibrato (MIDI CC#11), glide time, and attack time

Added real-time vibrato/portamento/attack time features to Sanjo Daegeum, Jungak Daegeum, and Danso.

Removed Nina articulation

Deleted the Nina articulation due to low usage.

Added Sustain articulation

Added sustain so notes are held while the key (or pedal) is pressed for Sanjo Daegeum, Jungak Daegeum, and Danso.

Version 1.6.0 (2024.10.24 16:42) — Added vibrato, portamento, attack time to select Strings libraries

Haegeum & Sanjo Ajaeng library update

Real-time vibrato (nonghyeon) control via MIDI CC#11 (Expression)

Added Glide Time (Portamento) connecting notes

Added Attack Time for a gradually increasing pitch effect (default 0)

Added MIDI note notation to Articulation display

Displayed Key Switch notes in the UI so playing methods are easier to identify.

Version 1.5.1 (2024.10.22 20:15) — Added sustain, GUI update, sample update

Woodwinds and select Strings — added Sustain function

Improved so notes sustain while holding the key (or pedal) for all woodwinds and for Sanjo Ajaeng, Jungak Ajaeng, Haegeum, etc.

Added articulation display in the UI

The current articulation is now displayed at the top of the woodwinds/strings UI.

Removed silence from fast Taepyeongso vibrato samples

Removed unnecessary silence at the beginning of fast vibrato samples to improve responsiveness.

Applied Round Robin to Samulnori janggu/kkwaenggwari

Applied Round Robin playback to produce more natural sound during repeated hits.

Version 1.4.7 (2024.10.10 17:05) — Fixed Saenghwang pitch error and Samulnori FX parameter bug

Fixed an issue where Saenghwang pitch could be inaccurate in certain ranges.

Fixed a bug where FX parameters were not applied in the Samulnori library.

Version 1.4.6 (2024.10.07 09:20) — Added user manual and EULA files

Packaged the manual & EULA files within the library folder to reflect newly added playing methods and license (EULA) changes after version updates.

Version 1.4.5 (2024.10.05 13:45) — Fixed Samulnori Expression bug

Fixed an issue where Expression did not apply correctly in some situations.

Version 1.4.4 (2024.10.02 19:10) — Added Geomungo articulations

Added support for new Geomungo articulations such as Ssaraeng, Jachul, Chuseong, etc.

Version 1.4.3 (2024.09.30 08:55) — Minor bug fix

Resolved errors related to “Maibeo” (Myber) by fixing exceptions occurring during internal parameter processing.

Version 1.4.2 (2024.09.28 16:20) — Added Sanjo Gayageum articulations

Added articulations such as Chuseong, Kkeokgi + Nonghyeon, Yeonnonghyeon, Yeontwigim, Gullym, etc., to increase expressiveness.

Version 1.4.1 (2024.09.25 11:45) — Added Jungak Gayageum articulations; added 25-string Gayageum tremolo

Added Jungak Gayageum “2x repeated pluck” articulation to expand performance options.

Improved the tremolo articulation for the 25-string Gayageum with enhanced sampling and expression.

Version 1.4.0 (2024.09.22 13:30) — Added 25-string Gayageum articulations

Expanded 25-string Gayageum articulations with 2x repeated pluck, 3x repeated pluck, Kkeokgi + Nonghyeon, Nonghyeon, Chuseong, etc., enabling diverse traditional Korean expressions.

Version 1.3.1 (2024.09.18 21:00) — Minor bug fixes

Fixed certain UI display issues and setting reset problems.

Version 1.3.0 (2024.09.15 14:10) — Major expansion of woodwind articulations and added Daepiri library

Major woodwind articulation expansion:

Sanjo Daegeum: Nira, Noniro, Crescendo, Daruchigi

Jungak Daegeum: Noniro, Crescendo

Dangpiri: Nira, Nire, Noniro, Nanireu

Sepiri: Nanireu, Nira, Nire, Nonireu

Hyangpiri: Nanireu, Nira, Nonireu, Toeseong, Chuseong, Deep Yoseong

Taepyeongso: Fast vibrato, Chuseong, Toeseong, velocity layer

Added Daepiri library:

Newly provided a dedicated Daepiri library that did not exist previously.

Version 1.2.1 (2024.09.14 09:50) — Minor bug fixes

Fixed issues occurring in some user environments during network updates.

Version 1.2.0 (2024.09.12 17:20) — Minor sample update and library additions

Adjusted Hyangpiri and Haegeum samples to improve noise and balance issues in specific ranges.

Added new woodwind libraries “Yak” and “Jeog” within the folder structure.

Experimentally introduced a server-based method for delivering update files by testing file transfer.

Version 1.1.2 (2024.09.10 11:05) — Bug fixes (resolved Windows and iOS partial instrument support issues)

Improved iOS compatibility

Fixed an issue where certain instruments were not supported on iOS.

Windows PC DS app instrument support patch

Updated compatibility so that woodwinds, samulnori, and other instruments that previously failed to load correctly in Windows environments now work properly.

Version 1.1.1 (2024.09.8 18:10) — Minor bug fixes

Minor stabilization: fixed small compatibility issues and some UI display errors.

Version 1.1.0 (2024.09.6 09:40) — Added “Ji” library (Woodwinds) and Platinum Bundle update

Added a standalone “Ji” woodwind instrument library.

Version 1.0.1 (2024.09.04 14:25) — Minor bug fixes; fixed Windows reverb error

Fixed an issue where reverb failed to load in Windows environments.

Fixed other minor issues occurring in some user environments.

Version 1.0.0 (2024.09.02 10:00) — Initial release

First release. This is the base version containing the initial features of the traditional Korean instrument libraries.
