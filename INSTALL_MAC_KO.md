# Widther 4.0.0 Beta 1 — macOS Apple Silicon 설치·평가

대상: Apple Silicon(arm64), macOS 11 이상, VST3 호스트, 48 kHz. AU·Intel Mac·44.1/96 kHz는 지원하지 않습니다. **평가·테스트용이며 공연·전시 현장 사용은 권장하지 않습니다.**

## 설치

1. [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1)에서 `Widther_4.0.0_macOS_arm64_48k_DREAMSCAPE_Inc_beta.zip`을 받습니다.
2. 터미널에서 `shasum -a 256 '<다운로드한 ZIP의 전체 경로>'`를 실행하고 [SHA256SUMS.txt](SHA256SUMS.txt)의 Mac 항목과 비교합니다. 다르면 설치하지 마세요.
3. DAW를 종료하고 ZIP을 풉니다. `Widther_4_0_0.vst3` 폴더 전체를 `~/Library/Audio/Plug-Ins/VST3/`에 복사한 뒤 DAW를 다시 시작하여 플러그인을 재검색합니다. 기존 버전과 프로젝트는 보존하세요.
4. 제조사 `DREAMSCAPE Inc.`와 `Widther 4.0.0`의 5ch/7ch Quality/Live 네 변형을 확인합니다.

## 안전한 평가 설정

- 프로젝트는 **48 kHz**, 플러그인이 들어간 트랙은 **12채널 출력**으로 설정합니다. 모노 소스를 입력 1번으로 보냅니다. 활성 출력은 선택한 5개 또는 7개뿐이며, 나머지는 무음입니다.
- 스피커를 연결하기 전에 낮은 후단 게인에서 `Output Check`로 출력 번호와 레벨을 확인하세요. 원음의 중복 라우팅을 피하고 Width/Diffuse 모드는 재생 전에 선택하세요.
- 신고 플러그인 PDC는 Quality 384 samples, Live 192 samples입니다. 호스트·오디오 인터페이스·공간 엔진 지연은 별도입니다.
- 이 ZIP은 Apple Developer ID 서명·공증이 없습니다. macOS 보안 정책이 로드를 막을 수 있으며, 시스템 보안 기능을 끄거나 경고를 무시해 설치하도록 권장하지 않습니다.

Apple Silicon CI에서 arm64 번들·16개 내장 뱅크·VST3 validator·25개 오디오 비교·네 GUI 뷰/제스처와 화면 캡처는 자동 검사했습니다. 그러나 **실제 Mac DAW 재생·프로젝트 저장/재열기·물리 출력 H006·청감·장시간 안정성은 아직 `not_run`**입니다. 현장 운용 승인이 아닙니다.
