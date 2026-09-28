# Widther 4.0.0 Beta 1 installation and evaluation

For Windows x64 VST3 hosts at 48 kHz. **Evaluation and testing only; live performance and installed-show use are not recommended.** Real DAW playback, saved-project recall, physical-output H006, listening evaluation, and an MSVC release build are still `not_run`.

## Install

1. Download `Widther_4.0.0_Windows_x64_48k_DREAMSCAPE_Inc_candidate.zip` from the [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1).
2. In PowerShell, run `Get-FileHash -Algorithm SHA256 -LiteralPath '<full path to downloaded ZIP>'` and compare it with [SHA256SUMS.txt](SHA256SUMS.txt). Do not install if they differ.
3. Close the DAW and extract the ZIP. Copy the **entire** `Widther_4_0_0.vst3` folder to `C:\Program Files\Common Files\VST3\`. Administrator approval may be needed. Preserve older versions and projects.
4. Reopen the DAW and rescan VST3 plug-ins. Check for manufacturer `DREAMSCAPE Inc.` and the four `Widther 4.0.0` 5ch/7ch Quality/Live variants.

## Safe evaluation setup

- Set the project to **48 kHz** and the plug-in track to **12 channels**. Feed the mono source to input 1. Outputs are muted at 44.1 and 96 kHz.
- The selected variant uses 5 or 7 active outputs; the remaining channels are silent. Route each active output to a distinct spatial-engine object input. Avoid duplicate dry-source routing.
- Start `Output Check` at its minimum level. Confirm channel order, polarity, and level before any physical speaker is connected; keep downstream gains low.
- Select Width / Diffuse M / Diffuse S before playback. Mode changes may briefly mute output. Changing modes during a show is outside this evaluation scope.
- Reported plug-in delay compensation at 48 kHz: Quality 384 samples, Live 192 samples. Host, interface, and spatial-engine latency are additional.
- The binary is not digitally signed. Windows may warn; verify its origin and SHA-256 before proceeding.

Real DAW playback, project save/reopen, physical H006, listening, and supported MSVC release-build gates are `not_run`. This beta is not approved for uninterrupted field operation.
