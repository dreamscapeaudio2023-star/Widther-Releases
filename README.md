# Widther 4.0.0 Beta 1

Widther is a mono-to-multichannel spectral width processor from DREAMSCAPE Inc. This repository contains public download instructions only; the VST3 binary is attached to the [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1), not committed to Git.

**Evaluation and testing only. Live performance and installed-show use are not recommended.** Automated checks have passed, but real DAW playback, saved-project recall, physical-output testing (H006), listening evaluation, and an MSVC release build have not been completed for this package. Do not treat this beta as a field-approved release.

- Windows x64 VST3; **48 kHz only**. At 44.1 or 96 kHz the plug-in mutes its outputs.
- Four plug-in variants: 5ch Quality, 5ch Live, 7ch Quality, 7ch Live. Each offers Width, Spectral Diffuse Medium, and Spectral Diffuse Strong as selectable modes.
- Mono input; host track requires 12 output channels. Only the chosen 5 or 7 active outputs carry signal. Route and identify each output before connecting speakers.
- The plug-in binary is not digitally signed; Windows may show a security warning. Verify the downloaded ZIP against [SHA256SUMS.txt](SHA256SUMS.txt) before installing.
- No source code, separate filter-bank WAV files, debug symbols, or internal research reports are provided in the download.

Install: [한국어 안내](INSTALL_KO.md) · [English guide](INSTALL_EN.md)

Copyright © 2026 DREAMSCAPE Inc.

---

Widther는 DREAMSCAPE Inc.의 모노 입력·다채널 출력 스펙트럴 Width 프로세서입니다. 이 공개 저장소의 Git 이력에는 안내 문서만 있으며, VST3 ZIP은 위 Pre-release의 다운로드 자산으로 제공됩니다.

**평가·테스트용 베타입니다. 공연·전시 현장 운용은 권장하지 않습니다.** 실제 DAW 재생, 프로젝트 저장·재열기, 물리 출력 H006, 청감 평가, MSVC 릴리즈 빌드는 아직 완료되지 않았습니다. 자동 검사를 통과했다는 사실이 현장 사용 승인이라는 뜻은 아닙니다.

Windows x64 / 48 kHz 전용이며 5ch·7ch의 Quality·Live 네 플러그인을 포함합니다. 호스트 트랙은 12채널로 설정하고, 실제 활성 출력 5개 또는 7개의 순서와 레벨을 스피커 연결 전에 확인하세요. 실행 파일에는 디지털 서명이 없으므로 다운로드 후 SHA-256을 확인하세요.
