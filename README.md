
# 2025 아이디어페스티벌 · 현장 투표 (GitHub Pages 패키지)

## 파일 구성
- `index.html` : 관객 투표(모바일)
- `stage.html` : 왼쪽 투표 주소(이걸로 QR 만드세요) + 오른쪽 실시간 결과(무대용)
- `teams_alias.csv` : 가명 팀 리스트 예시

두 HTML은 **같은 폴더**에 있어야 합니다. `stage.html`은 같은 폴더의 `index.html` 주소를 자동으로 표시합니다.

## GitHub Pages에 올리는 방법 (5분 컷)
1. GitHub에서 새 저장소(공개) 만들기. 예: `ideafest-vote`
2. 위 3개 파일을 저장소 **루트**에 업로드
3. `Settings` → `Pages` → `Source: Deploy from a branch`  
   `Branch: main / root` 선택 → **Save**
4. 1~2분 후 `https://<사용자이름>.github.io/ideafest-vote/` 주소가 활성화됩니다.

### 접속 주소
- 투표: `https://<사용자이름>.github.io/ideafest-vote/index.html`
- 무대: `https://<사용자이름>.github.io/ideafest-vote/stage.html`  
  (좌측 박스에 투표 주소가 자동 표시됨 → 이 주소로 QR 생성해서 스크린에 띄우세요)

## 사용법(데모)
1. 무대 PC에서 `stage.html` 열기(F11 전체화면)
2. 관객은 좌측 주소(혹은 QR)로 `index.html` 접속 후 투표
3. 우측 결과 그래프는 자동 갱신(데모는 localStorage 기반)
4. 실제 본선은 서버 연동(API)으로 집계 반영 필요
