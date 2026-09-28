# Widther 4.0.0 Beta 1 설치·평가 안내

대상: Windows x64 VST3 호스트, 48 kHz 프로젝트. **평가·테스트용이며 공연·전시 현장 사용은 권장하지 않습니다.** 실제 DAW 재생·프로젝트 재열기·물리 출력 H006·청감·MSVC 릴리즈 빌드는 아직 `not_run`입니다.

## 설치

1. [v4.0.0-beta.1 Pre-release](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1)에서 `Widther_4.0.0_Windows_x64_48k_DREAMSCAPE_Inc_candidate.zip`을 받습니다.
2. PowerShell에서 `Get-FileHash -Algorithm SHA256 -LiteralPath '<다운로드한 ZIP의 전체 경로>'`를 실행해 결과가 [SHA256SUMS.txt](SHA256SUMS.txt)의 값과 같은지 확인합니다. 다르면 설치하지 마세요.
3. DAW를 종료하고 ZIP을 풉니다. `Widther_4_0_0.vst3` **폴더 전체**를 `C:\Program Files\Common Files\VST3\`에 복사합니다. 관리자 권한이 필요할 수 있습니다. 기존 버전과 사용자 프로젝트는 덮어쓰거나 삭제하지 마세요.
4. DAW를 다시 열어 VST3를 재검색합니다. 제조사 `DREAMSCAPE Inc.` 및 `Widther 4.0.0`의 5ch/7ch Quality/Live 네 변형을 확인합니다.

## 안전한 평가 설정

- 프로젝트 샘플레이트를 **48 kHz**로, 플러그인 트랙을 **12채널**로 설정합니다. 모노 소스는 플러그인 입력 1번에 보냅니다. 44.1 및 96 kHz에서는 출력이 무음입니다.
- 선택한 플러그인의 활성 출력은 5개 또는 7개이며, 나머지 출력은 무음입니다. 각 출력을 공간 엔진의 서로 다른 오브젝트 입력에 직접 연결하고, 원음의 이중 라우팅을 피하세요.
- 물리 스피커를 연결하기 전에 `Output Check`를 최저 레벨에서 시작해 채널 순서·극성·음량을 확인합니다. 예기치 않은 큰 소리가 나지 않도록 출력 게인을 낮추세요.
- Width / Diffuse M / Diffuse S 모드는 재생 전에 선택하세요. 모드 전환 중 잠시 무음이 될 수 있습니다. 쇼 중 모드 전환은 평가 범위 밖입니다.
- 신고 PDC는 48 kHz에서 Quality 384 samples, Live 192 samples입니다. 호스트, 인터페이스, 공간 엔진 지연은 포함하지 않습니다.
- 바이너리는 디지털 서명되지 않았습니다. Windows 보안 경고가 나타날 수 있으며, 파일 출처와 위 SHA-256을 먼저 확인하세요.

실제 DAW 재생·프로젝트 저장/재열기·물리 H006·청감·MSVC 릴리즈 빌드 결과는 아직 `not_run`입니다. 이 베타를 무중단 현장 운용에 사용하도록 승인한 것이 아닙니다.
