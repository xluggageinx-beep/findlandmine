# Minesweeper 05I — Three Worlds

**최적화된 GitHub Pages 배포본**: 기존 5MB 이상의 인라인 이미지 데이터를 20개의 정적 이미지 파일로 분리해 `index.html`을 읽기 쉽게 만들고, 초기 HTML 파싱 비용과 화면 갱신 비용을 줄였습니다.

### 배포
1. ZIP 압축 해제
2. `index.html`, `audio/`, `assets/` 폴더를 GitHub 저장소 루트에 올리기
3. GitHub Settings > Pages > Deploy from a branch > `main` / `(root)`

### 기능
- 레트로, 연구실, 해적 테마와 배경음악 3곡, 2초 BGM 크로스페이드
- Web Audio API를 활용한 테마별 게임 효과음: 칸 열기, 깃발, SUCCESS, FAIL 폭발
- 스피커 1개로 BGM/SFX 함께 켜고 끄기, VOL 슬라이더로 둘 다 제어
- 이벤트가 발생한 칸만 갱신하는 속도 최적화; 연쇄 공개에 필요한 칸만 갱신
- PC 우클릭 / 모바일 길게 누르기 깃발 표시

효과음은 외부 효과음 파일을 사용하지 않고 Web Audio API에서 직접 합성합니다. 브라우저의 자동재생 방침에 따라 스피커 버튼을 눌러야 소리가 납니다.
