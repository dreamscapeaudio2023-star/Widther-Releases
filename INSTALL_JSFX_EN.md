# Widther 4.0.0 JSFX beta installation

For REAPER on Windows/macOS · **48 kHz only** · evaluation/testing only. Live or installed-show use is not recommended.

1. Keep backups of existing projects and earlier Widther folders; quit REAPER.
2. Use **Options → Show REAPER resource path in explorer/finder** to locate REAPER's resource directory.
3. Download `Widther_4.0.0_JSFX_Windows_macOS_48k_DREAMSCAPE_Inc_beta.zip` from the [v4.0.0-beta.1 release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1) and compare its checksum with `SHA256SUMS.txt`.
4. Copy the whole `Effects/Dreamscape/Widther_4_0_0` folder from the ZIP into `Effects/Dreamscape/` under the resource directory. Do not overwrite older version folders. The folder contains four FX, 16 WAV banks, and two images.
5. Restart REAPER and search its FX browser for `Widther 4.0.0`. Choose a 5ch/7ch Quality/Live variant, set the project to 48 kHz, connect a mono source to input 1, and set the track to 12 channels to inspect output pins.
6. Before connecting loudspeakers, identify outputs using Output Check at its minimum **−60 dBFS** level.

Each FX provides Width, Diffuse Medium, and Diffuse Strong as stopped-state modes. At 44.1/96 kHz or with fewer track channels than the active output count, output is muted. Native macOS REAPER loading and long physical-output testing of this JSFX package remain unverified. The JSFX processing text and WAV coefficients are readable public files. There is no automatic migration from VST3 or older JSFX projects.
