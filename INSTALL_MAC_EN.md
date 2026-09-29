# Widther 4.0.0 Beta 1 — macOS Apple Silicon installation

For Apple Silicon (arm64), macOS 11 or newer, VST3 hosts, and 48 kHz projects. AU, Intel Mac, 44.1 kHz, and 96 kHz are not supported. **Evaluation and testing only; live performance and installed-show use are not recommended.**

## Install

1. Download `Widther_4.0.0_macOS_arm64_48k_DREAMSCAPE_Inc_beta.zip` from the [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1).
2. Run `shasum -a 256 '<full path to downloaded ZIP>'` in Terminal and compare it with the Mac entry in [SHA256SUMS.txt](SHA256SUMS.txt). Do not install if it differs.
3. Quit the DAW and extract the ZIP. Copy the **entire** `Widther_4_0_0.vst3` folder to `~/Library/Audio/Plug-Ins/VST3/`, then reopen the DAW and rescan plug-ins. Preserve older versions and projects.
4. Confirm manufacturer `DREAMSCAPE Inc.` and four `Widther 4.0.0` variants: 5ch/7ch Quality/Live.

## Safe evaluation setup

- Set the project to **48 kHz** and the plug-in track to **12 output channels**. Feed a mono source to input 1. Only the selected 5 or 7 outputs are active; the others are silent.
- Before connecting speakers, use `Output Check` at low downstream gain to confirm output order and level. Avoid duplicate dry routing and select Width/Diffuse mode before playback.
- Reported plug-in delay compensation: Quality 384 samples, Live 192 samples. Host, audio-interface, and spatial-engine latency are additional.
- This ZIP has no Apple Developer ID signature or notarization. macOS security policy may block it. We do not recommend disabling system security protections or disregarding warnings to install it.

Native Apple Silicon CI automatically checked the arm64 bundle, 16 embedded banks, VST3 validator, 25 audio cases, four GUI views/gestures, and screenshots. **Actual Mac DAW playback, project save/reopen, physical-output H006, listening, and long-duration stability are still `not_run`.** This is not approval for field operation.
