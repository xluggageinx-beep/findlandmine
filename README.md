# Minesweeper — Three Worlds (05G)

레트로 / 연구실 / 해적 세 테마의 지뢰찾기 웹 게임입니다.

## 배포 방법 (GitHub Pages)

1. 새 **Public** 저장소를 생성합니다.
2. 이 ZIP 파일을 **압축 해제**합니다. (ZIP 파일 하나만 업로드하면 웹 게임이 실행되지 않습니다.)
3. 압축을 푼 파일 중 `index.html`, `audio/` 폴더(음악 3곡), `.nojekyll`, `README.md`를 **저장소 최상위(root)**에 업로드합니다.
4. GitHub 저장소 > **Settings > Pages** > **Build and deployment**에서 `Deploy from a branch`를 선택하고 `main / (root)`를 저장합니다.
5. Pages 배포가 완료되면 표시된 `https://<계정>.github.io/<저장소>/` 주소로 접속합니다.

### 파일 구조

```
index.html
.nojekyll
audio/
  retro.mp3
  lab.mp3
  pirate.mp3
```

브라우저 자동재생 제한 때문에 배경음악은 사용자가 `▶ 음악 재생`을 누르면 시작됩니다. 테마 변경 시 2초 크로스페이드, 반복 재생, 일시정지 및 볼륨 조절 기능을 지원합니다.

음원은 사용자가 제공한 레트로 `Iron Circuit`, 연구실 녹음 보정본, 해적 `Stormwind Armada`를 사용합니다. 웹 공개 전 각 음원의 서비스 약관과 공개·배포 권한을 확인하세요.
