# Widther 4.0.0 Beta 1 — VST3 and JSFX

Widther is a mono-to-multichannel spectral width processor from DREAMSCAPE Inc. This repository contains public download instructions only. VST3 and JSFX ZIPs are attached to the [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1), not committed to Git.

**Evaluation and testing only. Live performance and installed-show use are not recommended.** Automated checks have passed, but the published packages are not field-approved. Actual macOS DAW playback, project recall, physical-output testing (H006), listening evaluation, Developer ID signing, and notarization have not been completed. The original Windows package retains its previously documented test limitations.

- Windows x64 and native macOS Apple Silicon (arm64) VST3 packages; **48 kHz only**. At 44.1 or 96 kHz the plug-in mutes its outputs. AU and Intel Mac are not included.
- A separate REAPER JSFX package for Windows/macOS is also available. It is **48 kHz only** and uses the same four 5ch/7ch Quality/Live configurations and 16 unchanged float64 banks as the last JSFX runtime. Native macOS REAPER loading of this JSFX package has not yet been verified.
- Four plug-in variants: 5ch Quality, 5ch Live, 7ch Quality, 7ch Live. Each offers Width, Spectral Diffuse Medium, and Spectral Diffuse Strong as selectable modes.
- Mono input; host track requires 12 output channels. Only the chosen 5 or 7 active outputs carry signal. Route and identify each output before connecting speakers.
- The Windows binary is not digitally signed. The macOS package has no Apple Developer ID signature or notarization and may be blocked by macOS security policy. Do not disable system security protections to install it. Verify either ZIP against [SHA256SUMS.txt](SHA256SUMS.txt).
- The VST3 ZIPs do not provide source code or external filter-bank WAV files. **The JSFX ZIP necessarily exposes readable processing text and 16 filter-bank WAVs.** No internal research reports, private Git history, or user measurements are in the public repository or JSFX archive.

Install VST3: Windows [한국어](INSTALL_KO.md) / [English](INSTALL_EN.md) · macOS [한국어](INSTALL_MAC_KO.md) / [English](INSTALL_MAC_EN.md)

Install JSFX: [한국어](INSTALL_JSFX_KO.md) / [English](INSTALL_JSFX_EN.md)

Copyright © 2026 DREAMSCAPE Inc.

---

Widther는 DREAMSCAPE Inc.의 모노 입력·다채널 출력 스펙트럴 Width 프로세서입니다. 공개 Git 이력에는 안내 문서만 있으며, VST3와 JSFX ZIP은 위 Pre-release의 다운로드 자산으로 제공합니다.

**평가·테스트용 베타입니다. 공연·전시 현장 운용은 권장하지 않습니다.** Mac 실제 DAW 재생·프로젝트 재열기·물리 출력 H006·청감·Apple Developer ID 서명과 공증은 미실행입니다. Windows 패키지의 기존 미실행 항목도 유지됩니다. 자동 검사 통과는 현장 사용 승인이 아닙니다.

Windows x64와 macOS Apple Silicon(arm64)의 48 kHz VST3를 별도 ZIP으로 제공합니다. 5ch·7ch의 Quality·Live 네 플러그인을 포함합니다. 호스트 트랙은 12채널로 설정하고, 실제 활성 출력 5개 또는 7개의 순서와 레벨을 스피커 연결 전에 확인하세요. Mac ZIP은 Apple Developer ID 서명·공증을 받지 않았으므로 보안 정책상 로드가 차단될 수 있습니다. 설치 전 ZIP의 SHA-256을 확인하세요.

추가된 JSFX ZIP은 REAPER용 Windows/macOS 공용 48 kHz 베타입니다. JSFX 텍스트와 16개 필터 뱅크 WAV가 공개 파일로 들어 있으며, Mac REAPER 실제 로드는 아직 확인하지 않았습니다. [JSFX 설치 안내](INSTALL_JSFX_KO.md)를 읽고 기존 FX 폴더를 덮어쓰지 마세요.
