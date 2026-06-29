# sizenote-web

Size Note 앱의 공개 웹 페이지 — **개인정보처리방침 + 지원(Support) 페이지**.
앱 소스 코드(`SizeNote`, private)와 분리된 **공개 레포**입니다. 여기엔 정적 HTML만 있고 민감 정보는 없습니다.

## 파일
- `index.html` — 지원/소개 페이지 (App Store Connect "지원 URL"용)
- `privacy.html` — 개인정보처리방침 한/영 (App Store Connect "개인정보처리방침 URL"용)

## 게시 방법 (GitHub Pages, ~10분, 1회만)

1. GitHub에서 **새 public 레포** 생성: 이름 `sizenote-web`
2. 이 폴더를 push:
   ```sh
   cd "이 폴더"
   git init
   git add .
   git commit -m "Size Note 공개 웹 페이지 (PP + 지원)"
   git branch -M main
   git remote add origin https://github.com/jwparty/sizenote-web.git
   git push -u origin main
   ```
3. 레포 → **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / `/ (root)` → Save
4. 1~2분 후 게시됨. URL:
   - 지원: `https://jwparty.github.io/sizenote-web/`
   - 개인정보처리방침: `https://jwparty.github.io/sizenote-web/privacy.html`

## App Store Connect 입력
- **개인정보처리방침 URL** ← privacy.html URL
- **지원 URL** ← index.html URL (또는 루트)

## 내용 갱신
정본(SSOT)은 옵시디언 볼트 `05-PERSONAL-PROJECT/사이즈 지갑/docs/privacy-policy-2026-06-15.md`.
방침이 바뀌면 거기서 고친 뒤 `privacy.html`에 반영하고 다시 push하면 자동 재게시됩니다.
