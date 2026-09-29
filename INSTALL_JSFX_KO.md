# Widther 4.0.0 JSFX 베타 설치

대상: Windows/macOS의 REAPER · **48 kHz 전용** · 평가/테스트용. 공연·전시 현장 운용은 권장하지 않습니다.

1. 기존 프로젝트와 이전 Widther 폴더를 보존하고 REAPER를 종료합니다.
2. REAPER의 **Options → Show REAPER resource path in explorer/finder**로 리소스 경로를 확인합니다.
3. [v4.0.0-beta.1 릴리즈](https://github.com/dreamscapeaudio2023-star/Widther-Releases/releases/tag/v4.0.0-beta.1)에서 `Widther_4.0.0_JSFX_Windows_macOS_48k_DREAMSCAPE_Inc_beta.zip`을 받습니다. `SHA256SUMS.txt`의 체크섬과 비교하세요.
4. ZIP의 `Effects/Dreamscape/Widther_4_0_0` 폴더 전체를 REAPER 리소스 경로의 `Effects/Dreamscape/` 아래에 복사합니다. 다른 버전 폴더는 덮어쓰지 않습니다. 같은 폴더에 FX 4개, WAV 뱅크 16개, 이미지 2개가 있어야 합니다.
5. REAPER를 다시 열고 FX Browser에서 `Widther 4.0.0`을 검색합니다. 5ch/7ch × Quality/Live 중 하나를 고르고, 48 kHz 모노 소스를 입력 1에 연결합니다. 트랙 12채널을 설정해 각 출력 핀을 확인하세요.
6. 물리 출력 전에 Output Check를 최소 **−60 dBFS**에서 사용하여 출력 순서와 레벨을 확인합니다.

FX마다 Width, Diffuse Medium, Diffuse Strong을 정지 중 선택할 수 있습니다. 44.1/96 kHz 또는 활성 출력 수 미만의 트랙 채널에서는 안전 무음입니다. 이 JSFX의 실제 Mac REAPER 로드와 물리 출력 장시간 검증은 아직 완료되지 않았습니다. JSFX 파일과 WAV 계수는 읽을 수 있는 형태로 공개됩니다. VST3와 이전 JSFX 프로젝트의 자동 마이그레이션은 제공되지 않습니다.
