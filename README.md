# 병원 표준 임상용어집 검색 (배포용)

동물병원 차트용 임상용어 검색 페이지. **정적 사이트**(index.html 한 파일에 CSS·JS·데이터 내장).

> ⚠️ 병원 공식 승인본이 아니라 **검토용**입니다. 링크를 아는 사람은 누구나 접근 가능하므로
> 민감정보는 없어야 합니다. 검색엔진 노출은 robots.txt + meta noindex로 차단합니다.

## 배포 방법 (둘 중 하나)

### A. GitHub Pages (가장 간단)
1. 새 GitHub 저장소 생성 후 이 폴더의 파일(`index.html`, `robots.txt`, `.nojekyll`, `README.md`)을 push
2. 저장소 Settings → Pages → Source: `main` 브랜치 / `/ (root)` → Save
3. 몇 분 뒤 `https://<사용자명>.github.io/<저장소명>/` 으로 접속

### B. Render (Static Site)
1. GitHub에 위 파일 push
2. Render → New → Static Site → 저장소 연결
3. Build Command: (비움) · Publish directory: `.`
4. 배포 후 `https://<이름>.onrender.com` 접속

## 갱신
데이터/용어가 바뀌면 로컬에서 `python scripts/make_deploy.py` 재실행 → `index.html` 갱신본을
다시 push 하면 됩니다.
