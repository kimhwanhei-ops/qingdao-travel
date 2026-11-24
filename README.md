# QINGDAO 2027

정적 여행 페이지. 별도 프레임워크, 패키지 설치, 빌드, 서버가 필요하지 않습니다.

## GitHub Pages 배포
1. ZIP 압축 해제. `index.html`, `assets/`, `.nojekyll`, `README.md`가 있는 폴더의 **내용물**을 저장소 루트에 업로드합니다. 폴더 자체를 한 단계 더 중첩해서 업로드하지 마세요.
2. GitHub 저장소의 Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main → /(root) → Save.
3. Pages에서 제공하는 URL (예: `https://사용자명.github.io/qingdao-travel/`)을 친구에게 공유하세요. 실제 주소는 저장소명에 따라 다릅니다.
4. 모든 내부 파일은 상대 경로이므로 저장소명이 바뀌어도 됩니다. GitHub Pages 무료 계정에서는 일반적으로 공개 저장소를 사용합니다. 공개 사이트에는 여권 번호, 항공권 예약번호, 카드정보 등을 올리지 마세요. `noindex`는 접근 제한이 아닙니다.

공식 배포 문서: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 수정 및 실행
- `index.html`: 여행 정보·일정·매뉴얼·링크
- `assets/style.css`: 색상·반응형·인쇄 스타일
- `assets/app.js`: 체크리스트·날짜 탭·카운트다운·예산·복사
- `assets/images/`: 자체 제작 곤룡포풍 문양, 여행 엽서 일러스트, 파비콘
- `index.html`을 브라우저에서 열거나, 폴더에서 `python -m http.server 8000` 실행 후 http://localhost:8000 접속
- 체크리스트와 예산은 localStorage에 해당 브라우저별 저장됩니다. 두 사람 간 실시간 동기화 기능은 없습니다. 초기화 버튼은 기본 완료 항목을 유지합니다.
- 외부 사진은 Wikimedia Commons 원본 링크를 사용합니다. 네트워크 차단/실패 시 포함된 자체 제작 SVG가 그대로 표시됩니다. 사진 원본을 로컬에 다운로드해 묶지는 못했습니다. 원본을 직접 다운로드해 `assets/images/`에 두고 `data-photo` 값을 해당 상대 경로로 바꿀 수 있습니다.
- 사진 출처와 라이선스는 페이지 사진 하단에도 표시됩니다. Windmemories (잔교, 성미카엘 성당), Bbulussi (5·4광장), CC BY-SA 4.0: https://creativecommons.org/licenses/by-sa/4.0/ . 원본 사진은 자르기 표시 외 별도 수정하지 않았습니다.
- 여행 규정과 운영시간은 2026.11.24 기준 계획이며 2027년 1월 출발 전에 다시 확인하세요.
